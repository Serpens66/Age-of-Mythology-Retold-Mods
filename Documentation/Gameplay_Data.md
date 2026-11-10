# Gameplay data and additive mods

Use `game_current/game/data/gameplay/` for the installed base definitions.
The readable companions of `.XMB` files retain the inner filename. For field
semantics, see the shipped [Extended Core Data Guide](Sources.md#shipped-sources).
The archive and local mods establish paths, existing records and example syntax.

## Follow the data references

| Change | Inspect first | Follow next |
| --- | --- | --- |
| Unit, building, stats or unit group | `proto.xml`, `abstract_unit_types.xml`, `unit_type_data.xml` | ProtoAction names, `tactics/`, placement rules, asset and string IDs |
| Tech, unlock, relic or age progression | `techtree.xml`, `tech_types.xml`, `ages.xml` | Prerequisites, target kind, effect subtype, relativity and target unit or tech |
| Major god or culture | `major_gods.xml`, `minor_gods.xml`, `cultures.xml` | Age technologies, compendium and animations keyed by god or culture |
| Ability or god power | `powers.xml`, `abilities/abilities.xml` | Included `.abilities` or `.godpowers`, visible ability assignments, actions and targeting |
| Unit command or formation | `proto_unit_commands.xml`, `battle.xml` | Unit command references, UI, input context and hotkeys |
| Model or animation | ProtoUnit `animfile`, `simdata.xml` | AnimXML and referenced models, visual and synchronized animation data |

For example, the current `Hoplite` unit uses `handattack.tactics` and an
AnimXML under `greek/units/infantry/hoplite/`. It resolves its name through
`STR_UNIT_HOPLITE_NAME`. Its technology or availability may be defined
separately in `techtree.xml`. Placement rules have their own shipped reference,
and the repository's [Place Tower On Wall](<../Place Tower On Wall/game/data/gameplay/proto_mods.xml>)
shows a `placementfile` removal plus unit type and placement changes.

## Choose the additive entry point

Copy the directory shape under the mod root. The table lists entry points with
an official source or a concrete authored example. Use the filename and root
for that format, including exceptions to the usual suffix convention.

| Base | Mod file | Root or evidence |
| --- | --- | --- |
| `proto.xml` | `proto_mods.xml` | `protomods`. Local wall example above. |
| `techtree.xml` | `techtree_mods.xml` | `techtreemods`. [Passive Favor](<../Passive Favor (up to 60 per minute)/game/data/gameplay/techtree_mods.xml>) shows additional tech and effect records. |
| `proto_unit_commands.xml` | `proto_unit_command_mods.xml` | `protounitcommandsmods`. The additive filename uses singular `command`. [No Formation](<../No Formation/game/data/gameplay/proto_unit_command_mods.xml>) |
| `powers.xml` | `powers_mods.xml` | `powersmod` in the local Wandler experiment. Use its plural filename despite the singular filename in one section of the CryBar guide. |
| `abilities/abilities.xml` | `abilities/abilities_mods.xml` | `abilitiesmods`. Local Wandler experiment below. |
| `major_gods.xml` | `major_gods_mods.xml` | `civsmods` in the CryBar guide. Adding Major God IDs is officially supported. |
| `cultures.xml` | `culture_mods.xml` | Singular mod filename in the official notes. Use the installed structure and confirm the merge. |
| `simdata.xml` | `simdata_mods.xml` | `simdatabasemods` in the [WarHeroes example](<../WIP test/Unit - WarHeroes/game/data/gameplay/simdata_mods.xml>). Official additive support. |
| `strings/<language>/string_table.txt` | `strings/<language>/stringmods.txt` | Text records with `ID = "STR_MY_MOD_KEY" ; Str = "My text"`. The directory is under `game/data/`. |

[Current CryBar guide](https://github.com/CryShana/CryBarEditor/blob/main/Documentation/Modding.md) ·
[Additive God and Culture IDs](https://www.ageofempires.com/?p=136228) ·
[Additive SimData](https://www.ageofempires.com/news/age-of-mythology-retold-update-18-49472/)

The installed `powers.xml` includes both definition types from
`gameplay/god_powers/` and `gameplay/abilities/`. Add unique files and add their
`include` entries through `powers_mods.xml` when using that pattern. Then wire
the relevant tech, unit action or ability assignment. The Wandler test mod has
both pieces. Its comments about targeting and the number of visible abilities
are reports from earlier experiments. Re-test them for the relevant unit and
UI layout. Similarly, follow a ProtoUnit's `tactics` reference to a uniquely
named file when introducing new tactics. When overriding an existing
`.godpowers`, `.abilities` or `.tactics` resource, preserve its exact logical
name and verify which form the loader accepts. CryBar's guide shows repacking
the `.godpowers.XMB` override. A readable export is a reference copy.

[Wandler power includes](<../WIP test/Unit - Wandler/game/data/gameplay/powers_mods.xml>) ·
[Wandler ability assignments](<../WIP test/Unit - Wandler/game/data/gameplay/abilities/abilities_mods.xml>)

## Small first test

To exercise the ProtoUnit loader, put this in
`<ModName>/game/data/gameplay/proto_mods.xml` and enable the mod alone. On
19.17020 the base `House` has a `buildlimit` value of 16. Check that the fresh
merged ProtoUnit has the changed limit and that the intended culture's in-game
house placement reflects it. This patch is an authored test recipe.

```xml
<protomods>
  <unit name="House">
    <buildlimit mergeMode="replace">32</buildlimit>
  </unit>
</protomods>
```

## Merge matching evidence

Serp's merged CryBar contribution from October 2024 reports several distinct
matching behaviors. Treat the experiments as format-specific leads and
inspect the merged records on the current build before relying on them.
[Original PR change](https://github.com/CryShana/CryBarEditor/pull/10/changes/bda96850637c146a21bda611cb8a2c83fdc3ece7)

| Case | Use and evidence for 19.17020 |
| --- | --- |
| Appending a TechTree effect | Use explicit `mergeMode="add"` when adding an effect. A default modification can match an existing effect with identical outer attributes even if the nested target differs. In the installed tree, `MythicAgeHera` has an `Enable` effect for `Medusa`. Check that the original and added effects both survive. |
| Removing a flag by value | The PR reports that `<flag mergeMode="remove">NotSelectable</flag>` matched the value of a repeated tag. Verify this for the target node and that its other flags are unchanged. |
| Removing then adding a relic effect | `RelicAnkhofRa` currently has one `Data` / `ResourceTrickleRate` / `Favor` / `Absolute` effect, with amount **0.06**. A removal matching the PR's historical amount **0.05** is stale. Serp reported success omitting the numeric amount in a unique match. If using that approach, verify uniqueness in the current base and confirm that exactly one intended effect remains after the remove/add pair. |
| Selecting a repeated `protoaction` | The installed `VillagerEgyptian` has multiple actions including `RangedAttack`. The PR reports that putting the target action's nested `name` in the patch selected it and let the mod change `maxrange`. Confirm the merged action and surrounding actions. |
| Selecting a repeated `civ` | The PR observed an edit hitting the first `civ` instead of the intended sibling. Test a minimal patch against a non-first record before relying on nested matching. The official ability to add Major God IDs in newer builds addresses a different operation. |
| Inferring support from debug output | The PR used the data dump as a discovery aid. Confirm an additive filename through documentation or a minimal game test. Missing dump output does not establish that the format is override-only. |

The CryBar guide describes `modify`, `replace`, `remove` and `add`. Its examples
are a starting point. The exact matcher, behavior on ambiguous matches, number
of attributes that can be omitted, and whether a given `replace` changes
attributes are open per loader and record type. For a regression test, compare
the baseline, the mod in isolation and the mod with any overlapping package.
Check both the intended record and unrelated siblings. [Diagnostics](Mod_Workflow.md#verify-a-change)

The public notes also describe support for modded compendium history text and
matching of `learning_material_mods.xml` categories by name and topics by value.
New Major God or Culture IDs can become save and scenario dependencies. Verify
load with the original set of mods when testing that feature.
[Official 19.16313 modding notes](https://www.ageofempires.com/?p=136228)

## Local experiments to revisit

- **Tech lifecycle.** Gameplay Tweaks and Passive Favor explore `Volatile`
  techs with `OBTAINABLE` status as startup logic. Their comments report
  differences between new matches, campaign starts at an advanced age and
  loading saves, including an early `TypeCount` prerequisite failure. Re-test
  all intended entry points before adopting the pattern. A delayed effect may
  still have its prerequisite evaluated earlier.
  [Gameplay Tweaks tech experiments](<../WIP test/Gameplay Tweaks Serp/game/data/gameplay/techtree_mods.xml>)
- **Placement and socket ownership.** The wall experiments distinguish leaving
  the underlying wall, replacing it, and reverting to a socket after
  destruction. Check the placement result, ownership and rebuilding with the
  exact flags used in the new mod.
  [Gameplay Tweaks unit experiments](<../WIP test/Gameplay Tweaks Serp/game/data/gameplay/proto_mods.xml>)
- **Command wiring.** The No Formation mod links `researchTechInSelected`
  commands to tech entries. Local transform experiments tried alternate
  commands and ability paths with mixed results. Verify target ownership,
  single versus multi-selection and the active input context.
  [No Formation commands](<../No Formation/game/data/gameplay/proto_unit_command_mods.xml>)
