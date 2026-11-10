# Age of Mythology: Retold modding knowledge base

This repository documents the supported workflows for building Retold mods with
the game's data loaders, XS runtimes, Scenario Editor and model tools. The local
reference snapshot is Steam **23996698 / Retold 19.17020**. Read the snapshot page
before relying on build-specific names or values.

| Task | Start here |
| --- | --- |
| Install and activate a local mod, inspect merge results | [Mod workflow](Mod_Workflow.md) |
| Change a unit, tech, god, ability, command or gameplay asset reference | [Gameplay data](Gameplay_Data.md) |
| Understand a merge edge case from Serp's CryBar contribution | [Merge evidence and open questions](Gameplay_Data.md#merge-matching-evidence) |
| Write XS for triggers, maps or AI | [XS and scenarios](XS_and_Scenarios.md) |
| Look up differences in older XS or console documentation | [Doxygen comparison](XS_Reference_Differences.md) |
| Find an asset, model, UI image, localization or audio bank | [Assets and editor](Assets_and_Editor.md), [BAR inventory](BAR_Inventory.md) |
| Refresh Data.bar, the BAR inventory or the retail XS docs after Steam updates | [Local snapshot and refresh](Local_Snapshot.md) |
| Trace an assertion or compare the manuals with community examples | [Sources](Sources.md) |

Evidence terms used here:

- **Official** describes a shipped manual or a developer release note. Treat
  release notes as dated evidence and check for later superseding changes.
- **Data** establishes what a shipped file contains. **Static checked** means
  a path, identifier, signature or structure was checked against a file.
- **Example** describes how a repository or local mod is written. **Reported**
  describes an author's observation, with its source and build where known.
- **Open** marks an unresolved behavior. **Game tested** requires a recorded run
  with its build, active mods, mode and observed result. This baseline was
  verified statically.

When adding an entry, record the relevant file or source section and build.
Capture a reproducible test for uncertain behavior, then update the relevant
topic page with the result.
