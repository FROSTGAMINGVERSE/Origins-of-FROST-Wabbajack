# Origins Of FROST

A Nordic Skyrim modlist by **FROST FX**, built around Northern Roads, Ulvenwald and WardenWood, Bottled Shaders, BFCO combat, and grounded movement.

## Release status

**1.5.3 is a release candidate under validation.** This documents the current build, not a tested public download or Wabbajack Featured approval. The older 1.5.2 package does not reproduce this build. See [release gates](RELEASE-STATUS.md) and [changelog](CHANGELOG.md). Use a new game for candidate testing; save compatibility is not established.

## Requirements

- Windows 10/11 x64 and Steam Skyrim Special Edition with the Anniversary Upgrade's required Creation Club content downloaded in game.
- A Nexus Mods account and any free accounts required by the download sources. Premium is optional; downloads without Premium may require interaction.
- Microsoft Visual C++ 2015–2022 Redistributable x64.
- SSD storage. Enabled mods currently occupy approximately **242 GiB**, and source archives approximately **162 GiB**. Stock Game and temporary installation files require more space. Reserve **at least 500 GiB** for installation with downloads on the same volume; final compiler sizes will replace these planning estimates.
- Hardware minimums are not yet validated. 32 GiB RAM is a preparation recommendation, not a tested minimum. GPU/VRAM requirements depend on resolution and shader settings.

The runtime inside the list is **1.6.1170**, using an isolated **Stock Game** folder. Users must not manually downgrade or replace files in their Steam game as a prerequisite. Automatic reconstruction from supported storefront files must pass a clean-install test before release.

## Installation

These steps apply once a tested 1.5.3 package is linked in the release notes.

1. Install Skyrim through Steam, run its launcher once, and download the required owned Anniversary creations in game. Close Skyrim.
2. Install [Wabbajack](https://www.wabbajack.org/) and select the released Origins Of FROST package.
3. Choose an empty install folder outside Program Files, Steam's game directory, and OneDrive. Choose a downloads location with enough space; it may be on another drive.
4. Sign in to requested download services and finish installation. Resolve errors before launching.
5. Open the installed ModOrganizer.exe, select **Origins Of FROST**, and run **SKSE**.
6. Let first-launch shader compilation and new-game initialization finish before making a manual save.

Keep the supplied mod and plugin orders. Do not launch the list through Steam, use LOOT to replace its order, update individual shader/framework mods, or regenerate outputs as an ordinary installation step. The release should ship validated generated outputs.

## Included systems

- Northern Roads and its compatibility family receive late worldspace priority.
- Ulvenwald and WardenWood provide the forest setup.
- Bottled Shaders 1.0.27 with the Cabbage Effects11 setup supplies the current rendering configuration.
- BFCO, Modern Vanilla Combat, Elden Parry, and grounded movement shape combat.
- City, quest, armor, NPC, audio, UI and immersion additions retain their supplied compatibility patches.

Use the supplied profile INIs/configuration mods. A verified controls and MCM reference remains a release gate; no untested key bindings are asserted here.

## Known issues and limits

- Grass, terrain and object LOD must match the finalized road/forest setup; earlier output is not proof of a completed 1.5.3 generation run.
- Cabbage declares an unavailable lens-dirt resource with its intensity parameters set to zero. The unused-resource warning and final visual grading require verification.
- Startup is lengthy: previous warm tests were roughly two minutes on the development machine, not a guarantee for other systems.
- New-game initialization, save/load, travel, controls and sustained gameplay testing remain release gates. xEdit loading alone does not prove stability.

## Updates and support

Read the changelog before updating, back up saves/settings, and keep personal additions separate. Reproduce issues on the supported setup where possible.

Report bugs through [GitHub Issues](https://github.com/FROSTGAMINGVERSE/Origins-of-FROST-Wabbajack/issues), including release version, relevant errors, location and reproduction steps. Redact personal paths/account details before posting logs. The existing [community Discord](https://discord.gg/bPDhhyBej3) is an additional contact route. Support for the released list is not paywalled.

## Credits and reuse

Thanks to the original mod authors, Wabbajack, Mod Organizer 2, SKSE, xEdit, DynDOLOD, and all shader/patch/animation/asset creators. The [current enabled-mod inventory](MODLIST.csv) links upstream pages. The final compiled archive report will provide exact download attribution.

Original FROST-authored configuration and documentation may be forked, modified and redistributed under [LICENSE](LICENSE). Forks must use a distinct name and provide their own support. This does not grant redistribution rights over Bethesda files or third-party mods; their original licenses apply. Wabbajack must obtain their originals from appropriate sources and reconstruct permitted modifications.
