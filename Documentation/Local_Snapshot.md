# Local snapshot and refresh

Snapshot verified on **2026-11-10**. The Steam manifest for app 1934680 reported
build **23996698** and `AoMRT_s.exe` reported product version **100.19.17020.0**.
The matching public release is [Retold 19.17020](https://www.ageofempires.com/?p=136359).

## Local roots

- **Steam installation**: `E:\ProgrammeE\Steam\steamapps\common\Age of Mythology Retold`.
  Shipped manuals are under `BANG_Documentation`.
- **Modding directory**: `D:\CDesktopLink\Unterlagen\Mods\Age of Mythology Retold`.
  It contains `game_current`, `doxygen_retail`, `doxygen_old_aber_mehr`,
  previous `game_ab*` data snapshots, `mods/test`, and `tools`.
- **Player profile**: `%USERPROFILE%\Games\Age of Mythology Retold\<SteamID>`.
  Use the profile for the current account and launch mode. See [Mod workflow](Mod_Workflow.md).

| Installed input | Bytes | SHA-256 |
| --- | ---: | --- |
| `game/data/Data.bar` | 188,456,090 | `1b48a2268c183fd67e25ab7e9d0f1df418d5a0c642446b2e72a976de7b413e61` |
| `doxygen_retail.7z` | 342,987 | `2e77136b6b4ee4def98e0606fdd36ee6c912d93570de20f31747ee049eb2c7af` |

Resource Manager **0.7.0** supplied the BAR reader and decompressor for the
initial Data export through its installed .NET 8 x86 assembly. CryBar CLI
**1.3.20** listed all 64 BARs and converted the 327 XMB entries into readable
companions. Both the decompressed XMB files and their companions are available.
The checked `game_current/game/data/` tree contains **1,837 archive entries +
327 converted companions**. The Doxygen extract contains **51 files**, including
`index.html`. The install and the two extracts are local sources outside Git.

## Refresh after a Steam update

1. Read the product version and the Steam build ID. Hash the installed Data.bar
   and Doxygen archive. Compare the hashes with the last successful snapshot.
2. If Data.bar changed, use Resource Manager's **Extract All** on
   `game/data/Data.bar` into an empty stage. Preserve the internal root and
   subfolders, enable decompression, and keep the XMB inputs. For each XMB, use
   `crybar convert xmb-to-xml <input> -o <path-without-.XMB>` to add a readable
   companion. Preserve suffixes such as `.tactics` and `.godpowers` in the
   companion names. Stop if a companion would overwrite an existing member.
3. Compare the resulting paths with `crybar bar list <archive> --json`. Account
   separately for the companions. Parse the entire `proto.xml`, `techtree.xml`
   and `simdata.xml` as XML. Check the archive hash again before promoting the
   verified stage to `game_current`. Replace the previous directory as a unit
   so removed archive entries disappear. Keep the previous directory available
   for rollback until the new one is verified at its destination.
4. If the Doxygen hash changed, list it with `tar -tf <archive>` and extract
   with `tar -xf <archive> -C <empty-stage>`. Verify its file list and
   `index.html`, then replace `doxygen_retail` using the same staged approach.
   Open the new index and refresh the [older/retail comparison](XS_Reference_Differences.md)
   using function and variable summary tables as described there.
5. Re-list every installed BAR when refreshing the build inventory. Record any
   listing errors explicitly. Update this page and the [BAR inventory](BAR_Inventory.md).
   Review the [public release index](https://www.ageofempires.com/news/category/releases?game=aoem)
   and update relevant topic pages for currently usable features.

For the initial snapshot the XML roots were `proto`, `techtree` and
`simdatabase`. These checks establish integrity and provenance of the local
reference. Use a separate in-game test for load, merge and runtime behavior.
