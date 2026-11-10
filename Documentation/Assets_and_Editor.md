# Assets, UI, audio and editor tools

The [BAR inventory](BAR_Inventory.md) separates gameplay data from models,
textures, layouts, caches and sound definitions. Use CryBarEditor to locate
and selectively export dependencies. Version-specific tool capabilities are
described by the upstream project. This baseline used CryBar CLI 1.3.20 and
Resource Manager 0.7.0. The locally installed CryBarEditor folder is 1.0.7.
[CryBarEditor project and downloads](https://github.com/CryShana/CryBarEditor)

## Models, animations and visual effects

1. Read the shipped **ModelSystemModding**, **TMModel**, **Composite_Model**,
   **AnimXML**, **SimDatabase** and **Popcorn_VFX** manuals for the relevant
   part of the pipeline. Use `ArtImportFilesForModders.bar` for import
   descriptors and `ArtExamplesForModders.bar` for examples with FBX inputs.
2. Stage the FBX and matching `.fbximport` descriptors in a local mod. Add
   `.destructionimport` metadata when required. The official editor's
   **Objects > Model Convert Tool** writes `.tmm` and `.tmm.data` for models
   and `.tma` for animations. Use **Model Viewer** and **Model Visuals Debug**
   to inspect the output, skeleton, collision and animation references.
3. Wire the model through the relevant model manifest and AnimXML, and point
   the ProtoUnit to the AnimXML. Use the SimDatabase manual for `visual` and
   `animxml` records whose data can affect the simulation. Add only the
   required records through `simdata_mods.xml`. The public model update
   also documents `modelManifest_mods.xml` for model registration. Restart after enabling or
   disabling a model mod and inspect `mythlog.txt` for missing model,
   animation or bone references.

[Official PC model modding](https://www.ageofempires.com/news/age-of-mythology-retold-update-18-49472/) ·
[Model Viewer and Visual Debug](https://www.ageofempires.com/news/age-of-mythology-retold-update-18-56738/) ·
[AnimXML diagnostics](https://www.ageofempires.com/?p=136228)

For a material change, distinguish base color, normals and masks. The current
`ArtAtlanteanTextures.bar` listing shows DDT variants by asset and age.
CryBarEditor's DDT replacement workflow can retain source texture settings.
Check the exact material and variant the model uses.
[CryBar asset examples](https://github.com/CryShana/CryBarEditor/blob/main/Documentation/Modding.md#example-5-texture-changes)

## UI, localization and hotkeys

- The CryBar guide's older Hoplite icon example points to a PNG in
  `UIResources.bar`. On 19.17020, the listed member is
  `resources/greek/player_color/units/hoplite_icon.dds` in both
  `UITextureCache.bar` and `UITextureCache4K.bar`. The shipped ProtoUnit still
  references `resources\greek\player_color\units\hoplite_icon.png`. Distinguish
  this logical path from the DDS cache entry and its internal `intermediate/`
  root. Verify the actual mod override in the relevant texture modes. The
  19.14612 notes confirm god portrait overrides after the DDS transition.
  [Official DDS override fix](https://www.ageofempires.com/?p=136064)
- `UI.bar` contains XAML layouts and styles. Follow the actual resource
  reference for layout or icon changes. [No Formation](<../No Formation/game/data/gameplay/proto_unit_command_mods.xml>)
  demonstrates custom command icon paths and provides the images in its own
  `game/ui_myth/mod_icons/` tree. This is an authored example.
- UI text resolves through string IDs. Use the language directory and
  `stringmods.txt` for small localization changes. The 19.16313 notes
  describe English history entries under `game/data/strings/English/history/`,
  linked by learning material and table-of-contents data. For personal hotkeys,
  use the shipped Hotkey guide and profile `user.con`. Distinguish these
  bindings from modded default keymaps, command definitions and visible grid
  actions. Test the relevant input and UI mode.
  [Official history support](https://www.ageofempires.com/?p=136228) ·
  [Grid hotkey fix](https://www.ageofempires.com/?p=136331)

## Sound

Trace a ProtoUnit's `soundsetfile` to its action-to-soundset mapping. The
observed `Sound.bar` contains XMB definitions and a sound manifest. FMOD banks
are loose files under `game/sound/banks/Desktop/`. The localized German BAR
contains a separate manifest. Keep loose sound files, event/bank resources
and Scenario Editor sound references distinct. CryBar's sound instructions
include loose-file and custom soundset examples. Verify the actual event or
path, language, and runtime before reusing an older override example.
[CryBar sound examples](https://github.com/CryShana/CryBarEditor/blob/main/Documentation/Modding.md#working-with-sounds)
