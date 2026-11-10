# Installed BAR archive inventory

Snapshot: Steam build 23996698 / Retold 19.17020, inventoried 2026-11-10.
CryBar CLI 1.3.20 listed 64 archives. Entries below are archive-relative names.
The internal root is stored in the BAR header and is prepended on extraction (Data.bar uses
the root `game/data/`). The listed entries, folder counts and extensions are observed.
Descriptions describe likely use based on the member paths and shipped documentation.
Only Data.bar was extracted. The other 63 archives were listed without exporting members.

## game/art

| Archive | Entries | Internal root | Main member folders | Common extensions | Representative members | Use |
| --- | ---: | --- | --- | --- | --- | --- |
| `ArtAtlantean.bar` | 1,040 | `game/art/` | `atlantean` (1040) | `.xmb` (860), `.composite` (180) | `atlantean/buildings/armory/armory.xml.XMB` | Atlantean art assets |
| `ArtAtlanteanTextures.bar` | 1,661 | `game/art/` | `atlantean` (1661) | `.ddt` (1661) | `atlantean/buildings/armory/textures/armory_a_age2_matA_BaseColor.ddt` | Atlantean textures |
| `ArtAztec.bar` | 1,180 | `game/art/` | `aztec` (1180) | `.xmb` (940), `.composite` (240) | `aztec/buildings/armory/armory.xml.XMB` | Aztec art assets |
| `ArtAztecTextures.bar` | 1,866 | `game/art/` | `aztec` (1866) | `.ddt` (1866) | `aztec/buildings/armory/textures/armory_z_age2_matA_basecolor.ddt` | Aztec textures |
| `ArtBloodPack.bar` | 200 | `game/art/` | `bloodpack` (200) | `.composite` (103), `.xmb` (97) | `bloodpack/buildings/props/bone_pile_large_bloodied.xml.XMB` | BloodPack art assets |
| `ArtBloodPackTextures.bar` | 81 | `game/art/` | `bloodpack` (81) | `.ddt` (81) | `bloodpack/buildings/props/textures/bone_piles_animal_matA_basecolor.ddt` | BloodPack textures |
| `ArtChinese.bar` | 1,558 | `game/art/` | `chinese` (1558) | `.xmb` (1224), `.composite` (331), `.footprintimport` (3) | `chinese/buildings/armory/armory.xml.XMB` | Chinese art assets |
| `ArtChineseTextures.bar` | 1,923 | `game/art/` | `chinese` (1923) | `.ddt` (1923) | `chinese/buildings/armory/textures/armory_c_age2_matA_BaseColor.ddt` | Chinese textures |
| `ArtEffects.bar` | 106 | `game/art/` | `effects` (106) | `.tga` (75), `.xmb` (18), `.ddt` (13) | `effects/blue_noise/LDR_RGBA_64/LDR_RGBA_0.tga` | Effects assets |
| `ArtEgyptian.bar` | 1,043 | `game/art/` | `egyptian` (1043) | `.xmb` (819), `.composite` (224) | `egyptian/buildings/armory/armory.xml.XMB` | Egyptian art assets |
| `ArtEgyptianTextures.bar` | 1,315 | `game/art/` | `egyptian` (1315) | `.ddt` (1315) | `egyptian/buildings/armory/textures/armory_e_age2_matA_BaseColor.ddt` | Egyptian textures |
| `ArtEvents.bar` | 14 | `game/art/` | `events` (14) | `.xmb` (9), `.composite` (5) | `events/thanksgiving/buildings/props/relic/relic_turkey.composite` | Events art assets |
| `ArtEventsTextures.bar` | 15 | `game/art/` | `events` (15) | `.ddt` (15) | `events/thanksgiving/buildings/props/relic/textures/relic_turkey_mata_basecolor.ddt` | Events textures |
| `ArtExamplesForModders.bar` | 575 | `Tools/ExamplesForModders/` | `game` (574), `ModExamples` (1) | `.ddt` (201), `.fbx` (107), `.fbximport` (107), `.xmb` (101), `.destructionimport` (30) | `game/art/greek/buildings/house/house_g_a_age1.fbx` | Authoring examples including model source assets |
| `ArtGreek.bar` | 1,166 | `game/art/` | `greek` (1107), `greek_demeter` (59) | `.xmb` (925), `.composite` (241) | `greek/buildings/archery_range/archery_range.xml.XMB`<br>`greek_demeter/buildings/wonder/wonder_demeter.composite` | Greek art assets |
| `ArtGreekTextures.bar` | 2,065 | `game/art/` | `greek` (1947), `greek_demeter` (118) | `.ddt` (2065) | `greek/buildings/archery_range/textures/archery_range_age2_matA_BaseColor.ddt`<br>`greek_demeter/buildings/wonder/textures/wonder_demeter_matA_basecolor.ddt` | Greek textures |
| `ArtImportFilesForModders.bar` | 13,804 | `game/art/` | `japanese` (1856), `spc` (1821), `aztec` (1782), `chinese` (1689) | `.fbximport` (12818), `.destructionimport` (986) | `animation_library/TestCharAlignments/test_align_char_01.fbximport`<br>`atlantean/buildings/armory/armory_a_age2_damaged.destructionimport` | Model import descriptors shipped as references |
| `ArtJapanese.bar` | 1,512 | `game/art/` | `japanese` (1512) | `.xmb` (1035), `.composite` (262), `.destructionimport` (145), `.png` (63), `.mb` (6) | `japanese/buildings/ame_no_ukihashi/ame_no_ukihashi.composite` | Japanese art assets |
| `ArtJapaneseTextures.bar` | 1,801 | `game/art/` | `japanese` (1801) | `.ddt` (1801) | `japanese/buildings/armory/texture/armory_j_age2_mata_basecolor.ddt` | Japanese textures |
| `ArtLibraries.bar` | 69 | `game/art/` | `libraries` (69) | `.ddt` (69) | `libraries/textures/BuildingDecal_01/BuildingDecal_01_basecolor.ddt` | Shared art libraries |
| `ArtLighting.bar` | 23 | `game/art/` | `lighting` (23) | `.ddt` (18), `.cube` (5) | `lighting/blackball.ddt` | Lighting resources |
| `ArtMisc.bar` | 59 | `game/art/` | `misc` (58), `(archive root)` (1) | `.xmb` (44), `.tga` (10), `.composite` (4), `.json` (1) | `misc/background/chinese_map_background.material.XMB`<br>`changedDDTsOriginalDimension.json` | Misc art assets |
| `ArtMiscTextures.bar` | 125 | `game/art/` | `misc` (116), `(archive root)` (9) | `.ddt` (125) | `misc/background/texture/chinese_map_background_Mata_basecolor.ddt`<br>`black.ddt` | Misc textures |
| `ArtNature.bar` | 1,085 | `game/art/` | `nature` (1085) | `.xmb` (938), `.composite` (146), `.dd` (1) | `nature/animals/flying/dove/dove.material.XMB` | Nature art assets |
| `ArtNatureTextures.bar` | 1,163 | `game/art/` | `nature` (1163) | `.ddt` (1163) | `nature/animals/flying/dove/textures/dove_mata_BaseColor.ddt` | Nature textures |
| `ArtNorse.bar` | 1,023 | `game/art/` | `norse` (920), `norse_freyr` (103) | `.xmb` (785), `.composite` (238) | `norse/buildings/armory/armory.xml.XMB`<br>`norse_freyr/buildings/asgardian_hill_fort/asgardian_hill_fort.xml.XMB` | Norse art assets |
| `ArtNorseTextures.bar` | 1,366 | `game/art/` | `norse` (1267), `norse_freyr` (99) | `.ddt` (1366) | `norse/buildings/armory/textures/armory_n_age2_matA_BaseColor.ddt`<br>`norse_freyr/buildings/asgardian_hill_fort/textures/asgardian_hill_fort_age3_mata_basecolor.ddt` | Norse textures |
| `ArtShared.bar` | 1,142 | `game/art/` | `lightsets` (625), `shared` (517) | `.xmb` (983), `.composite` (149), `.png` (8), `.tga` (2) | `lightsets/04Open_Bluelight.lgt.XMB`<br>`shared/buildings/coal/coal.material.XMB` | Shared art assets |
| `ArtSharedTextures.bar` | 477 | `game/art/` | `shared` (477) | `.ddt` (477) | `shared/buildings/coal/textures/coal_mata_BaseColor.ddt` | Shared textures |
| `ArtSpc.bar` | 656 | `game/art/` | `spc` (656) | `.xmb` (509), `.composite` (146), `.bak` (1) | `spc/buildings/atlantis_tile/atlantis_tile.xml.XMB` | Scenario and campaign art |
| `ArtSpcTextures.bar` | 836 | `game/art/` | `spc` (836) | `.ddt` (836) | `spc/buildings/atlantis_tile/textures/atlantis_tile_pit_covered_matA_BaseColor.ddt` | Scenario and campaign textures |
| `ArtSpecial.bar` | 31 | `game/art/` | `special` (31) | `.xmb` (24), `.composite` (4), `.png` (3) | `special/tower_defence/basic_tower.xml.XMB` | Special art assets |
| `ArtSpecialTextures.bar` | 47 | `game/art/` | `special` (47) | `.ddt` (47) | `special/units/cheat/bella/textures/bella_mata_BaseColor.ddt` | Special textures |
| `ArtTerrain.bar` | 11 | `game/art/` | `terrain` (11) | `.xmb` (11) | `terrain/grass/long_grass/long_grass_1.material.XMB` | Terrain art assets |
| `ArtTerrainTextures.bar` | 1,572 | `game/art/` | `terrain` (1572) | `.ddt` (1572) | `terrain/atlantean/atlantean_beach_1_basecolor.ddt` | Terrain textures |
| `ArtUI.bar` | 585 | `game/art/` | `ui` (585) | `.ddt` (369), `.tga` (121), `.cur` (90), `.xmb` (5) | `ui/campaign_map/campaign_map_disolve_noise.ddt` | Art assets for the UI |
| `ArtVFX.bar` | 2,971 | `game/art/` | `vfx` (2971) | `.pkfx` (1709), `.composite` (649), `.xmb` (456), `.pkmm` (134), `.pkma` (14) | `vfx/blood/bleed.composite` | Visual effects assets |
| `ArtVFXTextures.bar` | 852 | `game/art/` | `vfx` (852) | `.ddt` (852) | `vfx/caustics/caustics_0000.ddt` | Textures used by visual effects |

## game/data

| Archive | Entries | Internal root | Main member folders | Common extensions | Representative members | Use |
| --- | ---: | --- | --- | --- | --- | --- |
| `Data.bar` | 1,837 | `game/data/` | `strings` (1493), `gameplay` (285), `map_definitions` (33), `trigger` (19) | `.txt` (1488), `.xmb` (327), `.xs` (18), `.blob` (3), `.cache` (1) | `gameplay/proto.xml.XMB`<br>`gameplay/techtree.xml.XMB`<br>`gameplay/simdata.xml.XMB`<br>`strings/English/string_table.txt` | Gameplay, localization and other data definitions |
| `fonts.bar` | 7 | `game/data/fonts/` | `(archive root)` (7) | `.ttf` (7) | `arialuni.ttf` | Font resources |
| `gamepad.bar` | 5 | `game/data/gamepad/` | `(archive root)` (5) | `.xmb` (5) | `cameramagnetismfilters.xml.XMB` | Controller resources |

## game/modelcache

| Archive | Entries | Internal root | Main member folders | Common extensions | Representative members | Use |
| --- | ---: | --- | --- | --- | --- | --- |
| `ArtModelCacheAnimationData.bar` | 6,794 | `intermediate/modelcache/` | `spc` (1441), `aztec` (977), `japanese` (964), `greek` (791) | `.tma` (6794) | `spc/buildings/dwarven_forge/anim/dwarven_forge_bellows_anim.tma`<br>`aztec/buildings/pillar_of_tlalocan/anim/pillar_of_tlalocan_birth_a.tma` | Cached model animation data |
| `ArtModelCacheMeta.bar` | 6,025 | `intermediate/modelcache/` | `chinese` (842), `japanese` (747), `aztec` (692), `greek` (681) | `.tmm` (6024), `.xmb` (1) | `chinese/buildings/armory/armory_c_age2.tmm`<br>`japanese/buildings/ame_no_ukihashi/ame_no_ukihashi.tmm` | Cached model metadata |
| `ArtModelCacheModelData.bar` | 1,203 | `intermediate/modelcache/` | `nature` (482), `spc` (328), `shared` (238), `bloodpack` (63) | `.data` (1203) | `nature/animals/flying/dove/dove.tmm.data`<br>`spc/buildings/atlantis_tile/atlantis_tile_pit_covered.tmm.data` | Cached model geometry (base) |
| `ArtModelCacheModelDataAtlantean.bar` | 671 | `intermediate/modelcache/` | `atlantean` (671) | `.data` (671) | `atlantean/buildings/armory/armory_a_age2.tmm.data` | Cached model geometry Atlantean |
| `ArtModelCacheModelDataAztec.bar` | 695 | `intermediate/modelcache/` | `aztec` (695) | `.data` (695) | `aztec/buildings/armory/armory_z_age2.tmm.data` | Cached model geometry Aztec |
| `ArtModelCacheModelDataChinese.bar` | 842 | `intermediate/modelcache/` | `chinese` (842) | `.data` (842) | `chinese/buildings/armory/armory_c_age2.tmm.data` | Cached model geometry Chinese |
| `ArtModelCacheModelDataEgyptian.bar` | 601 | `intermediate/modelcache/` | `egyptian` (601) | `.data` (601) | `egyptian/buildings/armory/armory_e_age2.tmm.data` | Cached model geometry Egyptian |
| `ArtModelCacheModelDataEvents.bar` | 6 | `intermediate/modelcache/` | `events` (6) | `.data` (6) | `events/thanksgiving/buildings/props/relic/relic_turkey.tmm.data` | Cached model geometry Events |
| `ArtModelCacheModelDataGreek.bar` | 686 | `intermediate/modelcache/` | `greek` (686) | `.data` (686) | `greek/buildings/archery_range/archery_range_age2.tmm.data` | Cached model geometry Greek |
| `ArtModelCacheModelDataJapanese.bar` | 747 | `intermediate/modelcache/` | `japanese` (747) | `.data` (747) | `japanese/buildings/ame_no_ukihashi/ame_no_ukihashi.tmm.data` | Cached model geometry Japanese |
| `ArtModelCacheModelDataNorse.bar` | 581 | `intermediate/modelcache/` | `norse` (534), `norse_freyr` (47) | `.data` (581) | `norse/buildings/armory/armory_n_age2.tmm.data`<br>`norse_freyr/buildings/asgardian_hill_fort/asgardian_hill_fort_age3.tmm.data` | Cached model geometry Norse |
| `ArtPhysCache.bar` | 986 | `intermediate/modelcache/` | `chinese` (155), `japanese` (145), `egyptian` (134), `greek` (126) | `.hkt` (986) | `chinese/buildings/armory/armory_c_age2_damaged.hkt`<br>`japanese/buildings/armory/armory_j_age2_damaged.hkt` | Cached physics model data |

## game/render

| Archive | Entries | Internal root | Main member folders | Common extensions | Representative members | Use |
| --- | ---: | --- | --- | --- | --- | --- |
| `Render.bar` | 37 | `render/` | `materialdefs` (34), `materials` (3) | `.xmb` (37) | `materialdefs/background.materialdef.XMB`<br>`materials/terrain_grass.material.XMB` | Render resources and shader inputs |
| `ShaderCacheDX12.bar` | 2,964 | `game/render` | `shader_cache_meta` (2964) | `.hlslc` (2964) | `shader_cache_meta/amd_ffx_debugvisualizeshadows_AMD_FFX_DebugVisualizeTilesCompute_cs_66694e6c8.hlslc` | Compiled DirectX 12 shader cache |

## game/sound

| Archive | Entries | Internal root | Main member folders | Common extensions | Representative members | Use |
| --- | ---: | --- | --- | --- | --- | --- |
| `Sound.bar` | 578 | `game/sound/` | `chinese` (81), `greek` (66), `japanese` (64), `aztec` (60) | `.xmb` (578) | `soundmanifest.xml.XMB` | Audio manifest and soundset definitions |

## game/sound_localized

| Archive | Entries | Internal root | Main member folders | Common extensions | Representative members | Use |
| --- | ---: | --- | --- | --- | --- | --- |
| `Sound-de-DE.bar` | 1 | `game/sound_localized/de-DE/` | `(archive root)` (1) | `.xmb` (1) | `soundmanifest.xml.XMB` | German localized sound manifest |

## game/ui

| Archive | Entries | Internal root | Main member folders | Common extensions | Representative members | Use |
| --- | ---: | --- | --- | --- | --- | --- |
| `UI.bar` | 305 | `game/ui_myth/` | `Content` (223), `Skins` (32), `SystemResources` (24), `Controls` (13) | `.xaml` (303), `.xmb` (2) | `Content/InGame/AgeUpPopup.xaml`<br>`Skins/Atlantean.xaml` | Core UI definitions and resources |
| `UI4K.bar` | 1 | `game/ui_myth_4k/` | `AppResources` (1) | `.xaml` (1) | `AppResources/4KBrushes.xaml` | High-resolution UI resources |
| `UIDefaultEditor.bar` | 251 | `game/ui_editor_default/` | `textures` (222), `(archive root)` (29) | `.tga` (125), `.ddt` (97), `.xmb` (28), `.dtd` (1) | `textures/background/background_black.ddt`<br>`button_sets.xml.XMB` | Default scenario editor UI |
| `UIEditor.bar` | 492 | `game/ui_editor/` | `textures` (463), `(archive root)` (29) | `.tga` (450), `.xmb` (28), `.ddt` (13), `.dtd` (1) | `textures/background/background_black.ddt`<br>`button_sets.xml.XMB` | Scenario editor UI |
| `UIResources.bar` | 33 | `game/ui_myth/` | `Fonts` (24), `resources` (9) | `.ttf` (24), `.cache` (9) | `Fonts/arialuni.ttf`<br>`resources/sdfprecache.cache` | UI fonts and signed-distance-field caches |
| `UITextureCache.bar` | 5,611 | `intermediate/uitexturecache/` | `resources` (5611) | `.dds` (5611) | `resources/greek/player_color/units/hoplite_icon.dds` | DDS UI textures including unit icons |
| `UITextureCache4K.bar` | 4,112 | `intermediate/uitexturecache4k/` | `resources` (4112) | `.dds` (4112) | `resources/greek/player_color/units/hoplite_icon.dds` | High-resolution DDS UI textures including unit icons |

## Loose files

- `game/random_maps/` contains shipped map scripts and metadata with reusable libraries.
- `game/ai/` contains the shipped AI scripts and their supporting data.
- `game/campaign/` contains campaign content outside the BAR inventory.
- `game/config/` contains game defaults such as `game.cfg`, `game.con`, and `editor.con`.
- `game/sound/banks/Desktop/` contains loose FMOD banks.

To locate a specific resource, run `crybar bar list <archive> --json` or browse the
archive in CryBarEditor. For an override, resolve the logical path from the
resource reference. A cache archive's internal root can differ from that path.
