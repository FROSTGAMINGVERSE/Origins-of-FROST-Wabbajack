# Origins Of Frost 2.0.2 Beta — community test

The [2.0.2 Beta installer](https://build.wabbajack.org/authored_files/download/Origins%20Of%20Frost%202.0.2%20Beta.wabbajack_ef5f4bf0-5356-4766-82cc-5eee7e0966d0) is available for community testing. Start a new game.

Completed: WardenWood and matching LOD resources, Ulvenwald fixes and texture fallbacks, mesh/material repairs, Forest Fragments updates, deliberate plugin cleaning, script fixes, and the all-world terrain/TexGen/DynDOLOD rebuild. xLODGen generated terrain only. TexGen HD Grass uses Direct 0, Ambient 100, Smoothness 0 for Community Shaders Grass Optimizations.

World coverage: all 20 worlds with their own supported LOD definitions were selected; 19 produced terrain files, while Shalidor's world has no LAND to generate. Nine worlds inherit LOD from generated parents. The remaining 49 world records have no own LOD definition. Bruma retains its author-specific LOD resources and occlusion handling.

Both display profiles now share gameplay and plugin order. The 16 protected character mesh/texture winners and SHA-256 hashes match in both profiles. Source archives and tool versions are recorded in Tools/SOURCES.json and the mod inventory.

## Known beta limitations

- Eleven existing door/navigation conflicts remain under repair. The authoring draft is preserved outside this package and is not enabled for gameplay.
- Visual tree and grass transitions, affected door travel/NPC navigation, and representative worldspace save/load tests are not yet verified for this revision.

Wabbajack verified the existing clean 2.0.2 reference installation. The public package retains the same hashes for every shipped file and drops 88 per-save test-state files. Both display profiles are included. The installer SHA-256 is `98cde86b537aecb05df3aaca43cf6de1711d9744d73d0db4e2a40ce85a9b230e`.
