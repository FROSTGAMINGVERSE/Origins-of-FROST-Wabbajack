# Changelog

## 2.0.0 Beta — Two-profile installer (2026-11-14)

- Added a separate 21:9 profile at 3440×1440, with native Vel’dun UI variants and profile-specific display settings. The standard 16:9 profile remains the default; gameplay and plugin order are shared.
- Updated the public installer link and its exact metadata/checksum for the 995,331,986-byte package.
- Tested a Wabbajack update of the existing Main Test installation using cached downloads: installer exit 0, native verifier 0 errors. All four pre-existing save files remained byte-identical.
- This is an existing-install update test, not a fresh empty-folder installation of this revision. In-game ultrawide validation, broad gameplay and final TexGen/DynDOLOD remain pending. Gallery registration still requires maintainer approval.


## 2.0.0 Beta â€” Compliance correction (2026-11-13)

- Clarified CC BY-NC-SA 4.0 for the compiled Wabbajack list and the separate MIT scope for original FROST documentation/configuration.
- Quarantined the custom patch, legacy Pandora, Leap Of Faith Fix and experimental Optiscaler bundles from compiler source downloads. Original source files are retained for rollback.
- Excluded the experimental Optiscaler DLSS 5 bundle and regenerable cell-offset caches from the release. The upscaling change needs a fresh runtime smoke test.
- Added targeted reconstruction companions for retained armor, combat bindings and Markarth overrides. Compilation and manifest verification are tracked separately; this entry does not claim an end-to-end install or broad gameplay test.
- Added the required AI-generated artwork tag and a specific creation/install disclosure on the Nexus artwork page. Legacy hosting retirement and Donation Points cleanup are tracked in the release status.

## 2.0.0 Beta â€” Gallery preparation (2026-11-13)

- Supersedes the released 1.5.2b baseline. The author selected the current setup for an as-is beta.
- Added compact 800x450 MO2 and 640x360 game launch splash screens, plus a new installer cover, in matching stone-and-steel Nordic branding.
- Added packaging companions for existing generated forest and ash material maps, with identical texture contents and reconstruction from original sources. Excluded a regenerable water-flow cache from the package.
- Audited embedded payloads against 1.5.2b and omitted lower-priority asset copies, optional developer symbols, backup files and the duplicate installed cover image. Winning game asset hashes are preserved; source mods remain intact.
- Compilation, archive integrity and scoped packaging checks passed. The slim package targets approximately 234 GiB installed and 177 GiB of source archives/game files; clean-install validation remains pending.

- Prepared the renamed Origins Of FROST profile for release.
- Categorized 14 additions without changing audited loose-file winners.
- Organized 15 plugin groups; collected 110 Northern Roads plugins/dependents late, with DynDOLOD.esm last among masters and DynDOLOD.esp/Occlusion.esp last among regular plugins.
- Compared 19,966 road/worldspace records through MO2-launched xEdit: 82 winners changed to the road compatibility family; static dependency checks passed. Full conflict/error and gameplay reviews remain pending.
- Retained Bottled Shaders 1.0.27 and preset compatibility fixes.
- Prepared isolated game files and a dedicated compiler catalog excluding locally archived ParallaxGen assets as download sources.
- Verified the isolated game reaches the main menu and a new character's starting room. The author confirmed save/reload and normal exit; Root Builder cleanup passed. The previous candidate was independently installed with zero verifier errors; broader gameplay and a fresh installation of the current corrected package remain pending.
- Updated requirements and documentation without claiming a completed public release.

Save compatibility is not established. Start a new game for candidate testing.

### Current C-base and unofficial gallery preparation

- Rebuilt from the independent C: installation. Removed the main-menu video requirement and added the static Skyrim Remastered wallpaper with compact wolf/dragon launch branding.
- Corrected PG source packaging: removed the hosted PG output dependency and rebuilt modifications from original sources. All 220,551 installed paths/hashes are unchanged.
- Corrected package is 1.08 GB; source downloads total about 174 GiB and installed directives about 233 GiB.
- Added matching installer metadata, checksum, packaging verification and a 16:9 gallery image. Prepared unofficial-gallery registration; public CDN upload and Wabbajack review are pending.

### Unofficial beta publication

- Uploaded the corrected installer to Wabbajack CDN. All upload response hashes and public definition matched; first, middle and last public chunk hashes passed.
- Prepared the numeric 2.0.0 gallery entry with an explicit Beta title, valid tags and matching metadata. Updated the public inventory to 1,948 enabled mods.
- Refreshed the repository landing page and current beta guide. Unofficial gallery approval and fresh corrected-package install testing remain pending.
