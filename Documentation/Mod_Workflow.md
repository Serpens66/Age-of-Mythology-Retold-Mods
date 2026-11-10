# Mod workflow and diagnostics

## Package and activate

1. Create a local test mod under
   `%USERPROFILE%\Games\Age of Mythology Retold\<SteamID>\mods\local\<ModName>`.
   Put the mod's files below its own `game/` subdirectory. Existing repository
   mods use `info.txt` for metadata and have a separate `game/` content tree.
   [Example metadata](<../Place Tower On Wall/info.txt>)
2. Mirror the resource's path as the game sees it. With CryBarEditor, set the
   installed `game` directory as the search root and the local mod folder as the
   export root. Keep reference exports such as a full vanilla proto in the local
   reference tree so they do not become incidental overrides.
   [CryBar modding guide](https://github.com/CryShana/CryBarEditor/blob/main/Documentation/Modding.md)
3. Use the in-game Mods screen to inspect and enable the local mod. Use a
   fresh game session after changing data or settings when validating behavior.
   Subscribed packages are a separate install route.
   [Retold scenario and mod installation](https://support.ageofempires.com/hc/en-us/articles/29922012212244-Scenario-Mods-Download-and-Installation-Instructions-Myth-Retold)
4. Prefer the supported additive filename for a small change. A whole-file
   override uses the resource's exact path and can conflict with another
   override of that file. Additive files can still conflict when they touch
   the same record or change a shared dependency. Compare with mods enabled
   in both relevant orders where precedence matters. The Mods Manager lists
   higher-priority mods nearer the top. [Official priority guide](https://support.ageofempires.com/hc/en-us/articles/29922620916756-What-does-the-mod-Priority-represent-Myth-Retold)

## Verify a change

- First verify the mod file is under the correct profile and package root.
  Check the filename, root element and current target record. Load the mod by
  itself and compare a fresh session with and without the mod.
- Use profile `config/user.cfg` for local settings and `config/user.con` for
  local bindings. The shipped Config/Hotkey guides explain their relation to
  `game.cfg` and `game.con`. The Steam ID folder and the `0` profile can
  have separate settings. [Shipped sources](Sources.md#shipped-sources)
- For additive diagnostics, try `DebugOutputGameData` and, for large files
  where needed, `+DebugOutputGameDataLargeFiles` in `user.cfg`. With the mod
  already enabled, restart and inspect fresh files under
  `%LOCALAPPDATA%\Temp\Age of Mythology Retold\Data`. Compare the generated
  record with the same-build baseline, then confirm the behavior in game.
  Output coverage varies. Its presence or absence is insufficient to infer
  support for an additive filename. [CryBar guide](https://github.com/CryShana/CryBarEditor/blob/main/Documentation/Modding.md#debugging-tips)
- Use `+DataValidation` and look in `mythlog.txt` for data/model warnings.
  Match the time and context of warnings to your test. Validation covers some
  lookups and parsing paths and can add load time. The public notes specifically
  describe duplicate editor object names and AnimXML lookup diagnostics.
  [Developer notes](https://www.ageofempires.com/?p=136228)
- Capture the build, enabled mods and order, active culture/DLC, scenario or
  save used, and the expected versus actual result. For simulation-affecting
  work, verify a same-build multiplayer session if that is a target, including
  how each participant obtains the content. Re-test saved games when a mod
  introduces IDs or dependencies. Replays have separate patch compatibility
  constraints. [19.17020 release notes](https://www.ageofempires.com/?p=136359)

The workspace notes also mention `generateTRConstants` as a way to discover
available symbolic values. The shipped Trigger guide places its output in
`%USERPROFILE%\Games\Age of Mythology Retold\temp\Logs`. That is a separate
location from the merged-data output.
