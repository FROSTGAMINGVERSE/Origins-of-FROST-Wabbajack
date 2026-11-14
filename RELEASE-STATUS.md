# 2.0.0 Beta release gates

The author selected the current setup for an as-is 2.0.0 Beta. The package compiled successfully and passed archive integrity and scoped packaging checks. The corrected beta installer is uploaded to Wabbajack CDN. Unofficial gallery registration is being submitted. Unchecked validation items describe known beta limitations and follow-up work, rather than claiming stable release readiness.

- [x] Active profile renamed; profile and instance configuration backed up.
- [x] Enabled mods and source archives inventoried.
- [x] Dedicated compiler recipe prepared with recovered artwork.
- [x] Current documentation and changelog drafted.
- [x] Stock Game copied; critical hashes and 74 required CC plugin files verified.
- [x] Stock Game launched through MO2; main menu and a new character in the Alternate Perspective starting room verified.
- [x] Author confirmed FROSTReleaseTest saves and reloads correctly, then exited normally; Root Builder reported clean.
- [ ] Current storefront-to-1.6.1170 automatic reconstruction verified.
- [x] Required source resolution and unmatched compiler files resolved; material maps reconstruct from original sources.
- [ ] Full plugin conflict/error review completed.
- [ ] Grass/terrain/TexGen/DynDOLOD outputs regenerated where required. TexGen and DynDOLOD explicitly deferred by the author on 2026-11-13.
- [x] Compiler completed; generated material maps use archive reconstruction, and scoped cache/personal-state and archive-integrity checks passed.
- [x] Previous v2.0 Beta installed into the empty C:\Games\Modded\Skyrim Test folder using copied archives; Wabbajack verifier reported 0 errors. This installation is the source of this rebuild; a second installation of the updated UI build is still pending.
- [ ] Controls, MCM configuration, final shader appearance, travel and sustained gameplay tested. The starting-room smoke test does not cover these checks.
- [ ] Measured requirements, final disk sizes and known issues finalized.
- [ ] Tested package and gallery metadata published.
- [ ] Unofficial gallery list supported for at least 30 days before Featured review.

Featured status is granted by Wabbajack after review, not by compilation.

## Earlier C-base rebuild — superseded

- Uses the independently installed C: profile, with the menu video removed.
- Wallpaper 1.1.0 and launch splash 1.0.0 are hosted on Nexus mod 135911, files 838021 and 838023.
- The approved MO2 splash is 800x450; the game-launch splash is 640x360.
- The fresh C-base cold launch recorded the main-menu event at 662.2 seconds (about 11 minutes), including first-launch initialization and shader compilation. All 2,250 plugins had loaded by about 7 minutes 19 seconds. Cold startup remains a known performance issue.
- Full gameplay, a fresh installation of this rebuilt package and visual confirmation of the new wallpaper remain pending.

## Earlier ParallaxGen-only candidate — superseded

- Removed Nexus mod 143468/file 768794 (hosted PG output) from compiler sources.
- PG output now uses 23,371 binary reconstruction directives and 311 unchanged sourced files; only its metadata file is embedded directly.
- All 220,551 installed paths/hashes match the previous candidate. ZIP CRC, native Wabbajack reader and native hash checks passed.
- Corrected installer: 1,075,602,242 bytes; metadata and verification are linked from the README.
- Fresh installation of this corrected candidate remains untested. CDN upload passed: public file definition and sampled public parts match. Unofficial repository review remains pending.

## Compliance correction — 13 November 2026

- Current corrected installer: 995,218,900 bytes; 2,107 source archives; 218,808 installed file directives. Four flagged bundle source dependencies and all packaged cell-offset caches are absent. Experimental Optiscaler DLSS5 is excluded.
- Retained overrides use original source downloads/reconstruction; no raw mesh/texture/DLL/HKX/PEX files are directly inlined. GPL notice and editable Papyrus binding interfaces are included.
- Public CDN definition and sampled chunk hashes match; all 475 upload responses matched.
- Nexus AI disclosures and standalone artwork presentation saved. Resources opted out of Donation Points. Clean optional configuration repair pack: mod143468/file838122. Archived historical content is not fully withdrawn; author declined contacting Nexus support. This remains a historical-hosting limitation, not a dependency of the corrected package.
- Fresh installation into C:/Games/Modded/Skyrim Compliance Test finished in 12 minutes 1 second using the existing downloads cache. Wabbajack native verify-modlist-install reported **0 errors**. No new gameplay, save/load, latest-storefront or final LOD validation is claimed.

## Current two-profile build — 14 November 2026

- Current package: 995,331,986 bytes; 2,107 source archives; 218,864 installed directives.
- Standard 16:9 and 21:9 3440×1440 profiles are included; default selection remains standard. Both use the same plugin/load order.
- Update installation into the existing Main Test folder completed successfully using cached sources. Native file verification found **0 errors**; four existing save files remained byte-identical.
- This revision has not been installed into a new empty folder or visually tested at 21:9 in game. Broad gameplay, startup performance and final TexGen/DynDOLOD remain pending.
- Unofficial registration remains at PR3949 awaiting Wabbajack maintainer review. Uploading a package does not grant gallery approval or Featured status.
