# Sources and research scope

## Shipped sources

All manual paths in this section are relative to the installed
`BANG_Documentation` directory. See [Local snapshot](Local_Snapshot.md) for the
source root and build. Prefer the manuals for intended behavior and current
installed data for concrete names, values and resource paths.

| Source | Use |
| --- | --- |
| `Data documentation/AoMRT_Comprehensive_Core_Data_Guide_Extended.pdf` and matching DOCX | Current bundled field reference. Credits Daniel Pereira, Eskiss and Tantalus and is dated 2026-06-25. The PDF's section starts are ProtoUnit p. 3, Tactics p. 28, ProtoUnitCommands p. 55, Major Gods p. 58, TechTree p. 68, God Powers p. 116 and Abilities p. 142. |
| `Data documentation/AoMRT Comprehensive Core Data Guide.pdf` | Earlier field reference. Resolve differences using the extended guide, current data and a targeted test. |
| `AoMRT_Placement_Rules_Documentation.txt` | Placement rule structure and examples. Preserve its distinction between parser-level findings and runtime questions. |
| `XS documentation` | Language, rules, coding standards, debugger, Doxygen and VS Code setup. |
| `Trigger documentation`, `RM documentation`, `AI documentation` | Supported syscall families, local setup and authoring workflows. |
| `Config documentation`, `Hotkey documentation` | Profile configuration and input bindings, including the distinction between Steam and non-Steam profiles. |
| `ModelSystem documentation` | Model conversion and registration, import metadata, composite models, AnimXML, SimDatabase and Popcorn VFX. |
Outside the manual directory, the installation ships Data.bar, other BARs,
loose game files, Doxygen and the VS Code extension. [BAR inventory](BAR_Inventory.md) ·
[Doxygen comparison](XS_Reference_Differences.md)

## Workspace sources

- The [existing Markdown Core Data Guide](<../AoMRT Comprehensive Core Data Guide Updated.md>)
  is a searchable older conversion. The repository's original README
  identifies known formatting and table problems. Use the shipped extended
  guide when resolving a cell or field definition.
- `info.txt` records local additive experiments, placement and ability leads,
  config switches and older installation paths. `info-scripting.txt` records
  XS setup, debug hotkeys and flags. The historical `MythTRConstants.txt`
  supplies names to cross-check, with values tied to its 2025-10-15 generation.
- Repo mods provide authored examples, while sibling `mods/test` and the repo's
  `WIP test` preserve experiments. In particular, read Gameplay Tweaks, Wandler,
  WarHeroes and the command/transform tests for leads on targeting, commands,
  model data and tactics. The icon mod folder provides UI material to inspect
  when needed. Local comments on limits and unfinished work remain reports.
- The local `game_ab_24_09_24` extract has `data/gameplay/simdata.simjson`.
  `game_aab_23_10_25` and the installed snapshot have `simdata.xml`.
  This confirms the practical format change for comparing old mods. The
  `game_ab*` snapshots and `doxygen_old_aber_mehr` are historical sources.

## Public sources used

| Source | How it informs the baseline |
| --- | --- |
| [Official Retold release index](https://www.ageofempires.com/news/category/releases?game=aoem) and [19.17020](https://www.ageofempires.com/?p=136359) | Match the installed build and check cumulative changes, mod compatibility, replay constraints and diagnostics. |
| [19.16313](https://www.ageofempires.com/?p=136228), [19.16764](https://www.ageofempires.com/?p=136331), [19.14612](https://www.ageofempires.com/?p=136064) | Additive IDs, compendium, editor tools, grid hotkeys and DDS overrides. |
| [18.49472](https://www.ageofempires.com/news/age-of-mythology-retold-update-18-49472/), [18.56738](https://www.ageofempires.com/news/age-of-mythology-retold-update-18-56738/) | Model conversion, model manifests, SimData and Model Viewer. |
| [CryBar modding guide](https://github.com/CryShana/CryBarEditor/blob/main/Documentation/Modding.md) and [Serp's Oct 2024 contribution](https://github.com/CryShana/CryBarEditor/pull/10/changes/bda96850637c146a21bda611cb8a2c83fdc3ece7) | Author reports and examples for package paths, additive entry points, repeated records, XMB, asset overrides and diagnostics. Compare against the installed build before treating an example as current. |
| [CryBar release and CLI](https://github.com/CryShana/CryBarEditor/releases/tag/1.3.20) and [Resource Manager v0.7 announcement](https://forums.ageofempires.com/t/v-0-7-resource-manager-age-of-myth-retold-bar-extractor/260136) | Archive and conversion tooling. |
| [AoMR modding wiki](https://github.com/aomr-mod-dev/aomr-mod-dev.github.io/wiki) and [Liam Appelbe's map tutorial](https://liamappelbe.medium.com/aomr-random-map-scripting-fbe62b60f46a) | Additional XS examples and random-map workflow. |
| [Age of Empires III DE additive guide](https://support.ageofempires.com/hc/en-us/articles/360062106732-Additive-Data-Mods) | Related engine background referenced in local notes. Use Retold evidence for loader details, tags and supported filenames. |
