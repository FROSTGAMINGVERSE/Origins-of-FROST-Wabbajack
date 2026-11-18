# Origins Of Frost 2.0.2 Beta — private candidate

This package is undergoing validation. It has not been published as a completed release.

Completed: WardenWood and matching LOD resources, Ulvenwald fixes and texture fallbacks, mesh/material repairs, Forest Fragments updates, deliberate plugin cleaning, script fixes, and the all-world terrain/TexGen/DynDOLOD rebuild. xLODGen generated terrain only. TexGen HD Grass uses Direct 0, Ambient 100, Smoothness 0 for Community Shaders Grass Optimizations.

World coverage: all 20 worlds with their own supported LOD definitions were selected; 19 produced terrain files, while Shalidor's world has no LAND to generate. Nine worlds inherit LOD from generated parents. The remaining 49 world records have no own LOD definition. Bruma retains its author-specific LOD resources and occlusion handling.

Both display profiles now share gameplay and plugin order. The 16 protected character mesh/texture winners and SHA-256 hashes match in both profiles. Source archives and tool versions are recorded in Tools/SOURCES.json and the mod inventory.

Release holds:

- Eleven existing door/navigation conflicts remain under repair. The authoring draft is preserved outside this package and is not enabled for gameplay.
- Visual tree and grass transitions, affected door travel/NPC navigation, and representative worldspace save/load tests are not yet verified for this revision.
- Compilation and fresh-install verification must be recorded against the exact resulting installer hash.

Desktop control was recovered during the 18 November compiler pass. Remaining Creation Kit navigation and visual runtime checks are still required. A successful compilation or file verification alone does not remove those holds. No Nexus, CDN or release-index update has been performed for this candidate.
