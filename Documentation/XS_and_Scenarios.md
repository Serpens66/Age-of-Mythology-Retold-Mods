# XS, maps, AI and scenarios

Start with the shipped `BANG_Documentation/XS documentation` manuals for
syntax, rules, coding standards and debugging. Extract the official VS Code
extension from `vscodeextensionretail.7z` and install its VSIX from the editor's
Extensions menu if using VS Code. Open `doxygen_retail/index.html` to check
types, arguments and available comments. Use the shipped scripts to establish
which runtime and entry point the code belongs to. [Source map](Sources.md#shipped-sources)

## Choose the runtime

| Work | Starting point | API and test setup |
| --- | --- | --- |
| Scenario and trigger code | Scenario Editor and its Trigger guide. Follow the scenario's existing script or trigger entry point. | XS, TR and KB syscalls. Use `debugTriggers`, `enableTriggerEcho` and `generateTRConstants`. Test in editor playtest and the intended scenario launch path. |
| Random map | Installed `game/random_maps/air.xs` and `air.xml` are a paired example. Inspect `game/random_maps/lib/` for shared code. Package custom files under the mod's `game/random_maps/`. | XS, RM and KB syscalls. Use `debugRandomMaps` and `generateRMConstants`. Reproduce a failure with its seed, then test different seeds, player counts and map sizes. |
| Skirmish AI | Installed `game/ai/chairon.xs` and `game/ai/personalities/`. Follow the shipped AI guide for the entry point and personality registration. | XS, AI and KB syscalls. Use the documented `aiDebug` setting for debug tools and `generateAIConstants` where needed. Test as a controlled AI slot and inspect plans and logs. |

[Developer random-map walkthrough](https://liamappelbe.medium.com/aomr-random-map-scripting-fbe62b60f46a) ·
[Community XS examples](https://github.com/CryShana/CryBarEditor/blob/main/Documentation/XSScriptingReference.md)

Keep local debug settings in profile `config/user.cfg` and bindings in
`config/user.con`. The shipped XS debugger guide documents the default
`Alt+Shift+D` binding, runtime switching, breakpoints, call stack and variable
inspection. The RM guide covers same-seed and new-seed reloads. The documented
constant output is under `%USERPROFILE%\Games\Age of Mythology Retold\temp\Logs`.
Regenerate constants when testing the installed build or a modded database.
The workspace `MythTRConstants.txt` is dated 2025-10-15 and is a historical
symbol index.

## Find and validate a syscall

- Read the declaration and function comments in the relevant retail page.
  Shared XS and KB pages supplement the runtime-specific TR, RM and AI pages.
  Keep selection, unit IDs, ProtoUnit IDs and the current player context
  distinct. The local research-all-techs snippet illustrates the relationship
  between `xsSetContextPlayer(int playerID)`, the
  `kbTechTreeGetAllObtainableTechnologies(bool needAliveResearcher)` query, and
  `trTechSetStatus(int playerID, int techID, int status)`. Those signatures
  are present in retail. The broad state-changing snippet remains an example
  to verify in an isolated scenario.
- Use the [older/retail comparison](XS_Reference_Differences.md) for additional
  leads. The old snapshot exposes console and UI pages absent from retail.
  For example, the older page lists `uiTransformSelectedUnit`, while local
  command experiments reported a button that did nothing. A name in an old
  console list does not establish that it can be called from a ProtoUnit
  command, hotkey or XS runtime. Test the exact context separately.
- Check current release notes where an API is absent or ambiguous. For example,
  the current retail Doxygen lists `trBoxFormationSpacing(float minUnitRadius)`,
  and the 19.16313 notes describe its use in the editor's Box Formation trigger.
  [Official 19.16313 notes](https://www.ageofempires.com/?p=136228)

## Scenario workflow

Keep the scenario's dependencies with the local package, test its intended
start and save/load paths, and verify player ownership and trigger context.
When the target is multiplayer, check transfer and whether every player needs
the mod's additional files. A scenario transferring successfully establishes
that scenario's behavior only. The 19.16313 notes document improvements to
large map transfer and editable human/AI slot states in custom lobbies.
The local note about very deep terrain deleting projectiles remains open for
the current build. [Official scenario and editor notes](https://www.ageofempires.com/?p=136228)
