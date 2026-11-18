# Origins Of Frost 2.0.2 Beta

A Nordic Skyrim modlist by **FROST FX**, built around Northern Roads, Ulvenwald and WardenWood, Bottled Shaders, BFCO combat and grounded movement.

**Working candidate: the new installer is not published yet.** Native generation, runtime review and a fresh installation are separate checks. Their results will be recorded for this exact package before publication. Earlier installers and historical tests do not establish acceptance of this revision. See [release status](RELEASE-STATUS.md) and the [changelog](CHANGELOG.md).

## Requirements

- Windows 10/11 x64 and Steam Skyrim Special Edition with the required owned Anniversary Upgrade creations downloaded in game.
- A Nexus Mods account and Microsoft Visual C++ 2015â€“2022 Redistributable x64. Nexus Premium is optional; free downloads can require interaction.
- SSD space for the installed list, source archives and installation workspace. Exact sizes accompany the validated installer.
- Hardware requirements and sustained performance remain under testing; resolution and shader settings affect memory use and frame rate.

The list uses an isolated **Skyrim 1.6.1170** runtime. Wabbajack reconstructs the supplied game files from owned sources. Do not manually downgrade Steam as an installation prerequisite. **Start a new game:** save compatibility is not established.

## Installation

1. Install Skyrim through Steam, run its launcher once and download the required owned Anniversary creations in game. Close Skyrim.
2. Open the matching Origins Of Frost installer in [Wabbajack](https://www.wabbajack.org/).
3. Choose an empty installation folder outside Program Files, Steam and OneDrive. Choose a downloads folder with enough free space.
4. Sign in to the requested download services and let installation finish. Resolve installation errors before launching.
5. Open the installed `ModOrganizer.exe`, select a display profile and run **SKSE**. Root Builder manages the launch-time game-root files.
6. Allow first-launch shader compilation and new-game initialization to finish before making a manual save.

Both profiles install together and share gameplay and plugin order:

| MO2 profile | Display configuration |
| --- | --- |
| Origins Of Frost | Standard 16:9, 3840 Ã— 2160 |
| Origins of Frost 21x9 | Ultrawide, 3440 Ã— 1440, with its interface configuration |

Choose the profile in MO2 after installation. Keep the supplied mod and plugin orders. Individual mod updates, automatic LOOT sorting and output regeneration are maintainer changes that require renewed validation. Players receive the completed outputs and do not need to run the generators.

## Included setup

The character defaults use a fixed Nordic female body preset, vanilla female underwear, HIMBO Natural with linen underwear, and the accepted character and clothing physics settings. OBody distribution is retired. Character mesh, underwear and skin settings are protected during scenery maintenance.

The scenery rebuild updates WardenWood and its matching 3D LOD resources, Forest Fragments and its Falkreath patch, Ulvenwald snow-log fixes and DynDOLOD runtime support. Bark and pine-branch fallbacks cover intentional vanilla texture paths. Compatibility repairs retain the original source downloads as installer dependencies.

The maintenance sequence is **source repairs and deliberate plugin cleaning â†’ PGPatcher â†’ xLODGen terrain only â†’ TexGen â†’ DynDOLOD**. Terrain generation excludes objects, trees and occlusion. DynDOLOD handles object and tree LOD, dynamic LOD, optimized grass assets and the separate occlusion plugin for supported worlds.

Grass LOD follows Community Shaders Grass Optimizations: TexGen HD Grass **Direct 0, Ambient 100, Smoothness 0**, followed by DynDOLOD CS Optimized Grass assets. Nearby grass lighting is preserved. Bruma retains its author-specific LOD and occlusion handling, with its compatibility resources winning after generated outputs.

Maintenance tools have readable MO2 labels. Their versions, original downloads and settings are documented in `Tools/README.txt`, `Tools/SOURCES.json` and the [tree and LOD maintenance notes](compatibility/TREE-LOD-MAINTENANCE.md). Local development connectors, credentials, logs and shader caches are excluded from the player package.

## Beta testing and support

Generator completion, native plugin checks, file verification and runtime tests cover different failure modes. They do not establish that every quest, location or gameplay combination is free of bugs. The release record identifies tested worlds, save/load checks and remaining limitations.

First startup can be lengthy while shaders and caches build. Historical cold launches took approximately eleven minutes on the development machine; this is an observation, not a performance guarantee. Allow progressing initialization to finish.

Report reproducible issues through [GitHub Issues](https://github.com/FROSTGAMINGVERSE/Origins-of-FROST-Wabbajack/issues), including the release version, location, error and reproduction steps. Remove personal paths and account details before posting logs. The existing [community Discord](https://discord.gg/bPDhhyBej3) is another support route. The list and support are free; donations never gate access.

## Credits and reuse

Thanks to the original mod authors and the Wabbajack, Mod Organizer 2, SKSE, xEdit, DynDOLOD, shader, patch, animation and asset developers. The [enabled-mod inventory](MODLIST.csv), source records and compiled archive report provide upstream attribution.

Standalone FROST menu artwork is on [Nexus mod135911](https://www.nexusmods.com/skyrimspecialedition/mods/135911). Owned list configurations are on [Nexus mod143468](https://www.nexusmods.com/skyrimspecialedition/mods/143468); the matching installer installs them automatically. The artwork uses AI-assisted image generation, disclosed on its source pages.

The compiled Wabbajack modlist is **CC BY-NC-SA 4.0**. The separate MIT grant in [LICENSE](LICENSE) covers original FROST-authored configuration and documentation only. Bethesda files and third-party mods retain their original terms. These grants do not authorize rehosting their assets. Processed third-party meshes and cleaned official plugins are reconstructed from original downloads or owned game files.
