# Tree and grass maintenance record — 17 November 2026

This records the current development rebuild. Terrain, TexGen and DynDOLOD generation and output checks completed.
Navigation repairs, gameplay acceptance and fresh installation remain release gates.

The plugin shown as a tree's last editor does not identify the winning mesh or
texture. MO2's loose-file priority, archived assets, generated meshes and Base
Object Swapper can each affect the rendered tree independently of that label.

The installed WardenWood source was older than the V1.5 author release. Its new
release fixes the shader on `treepineforestdead06` and `treepineforestdead07`,
updates texture mipmaps and improves 3D LOD support. The source and matching
author LOD archive have been updated. Ulvenwald's current main and 3.3.2b fixes
were already installed. The separate author Snow Logs FIX is now installed.

Some Ulvenwald logs and driftwood intentionally use vanilla texture paths.
Texture-only bark and pine-branch fallbacks sit below the tree overhauls, so
they improve those paths without displacing the overhauls' custom textures.

An unused-looking Sleeping Tree alias under `Ash Forest` referenced missing
`sacredbark01_c.dds` and `sacredbark01_glow.dds`. The local repair uses Ulvenwald's
working canonical Sleeping Tree mesh at that alias, with its valid bark paths.
It does not supply unrelated textures under invented names.

The WardenWood V1.5 LOD archive contains three checksum filenames that do not
match the V1.5 full source meshes: pine ash 02, dead snow 02 and dead snow 04.
Checksum aliases are staged from the author's corresponding LOD meshes. Their
mesh bytes remain identical to the author archive. The other 87 checked LOD
filenames match their corresponding source checksums. Final DynDOLOD reports contain no missing-model generation errors.
In-game swap and LOD transitions still require visual acceptance.

The supplied WardenWood preset is retained as an author reference. It contains
machine-specific paths and limited world selections. Do not blindly substitute
it for the list's generation settings. The author acknowledges that some
complex BOS swaps can still differ between nearby trees and LOD. Test these
transitions in game, including snow and Solstheim trees.

The grass correction concerns LOD only. This list uses Community Shaders Grass
Optimizations. Its documented TexGen HD Grass settings are Direct 0, Ambient
100 and Smoothness 0; DynDOLOD must then create the CS Optimized Grass assets.
Nearby grass lighting and the accepted shader preset remain unchanged.

Sources: [WardenWood files](https://www.nexusmods.com/skyrimspecialedition/mods/197013?tab=files),
[author discussion](https://www.nexusmods.com/skyrimspecialedition/mods/197013?tab=posts),
[Grass Optimizations workflow](https://dyndolod.info/Mods/Community-Shaders),
[BOS handling](https://dyndolod.info/Mods/Base-Object-Swapper).

Native tree audit: 2,509 model paths were checked. The three absent Ulvenwald
base models (BirchTree03 and DogwoodTwisted01/03), and Falkreath center-tree
replacer's dry variant 802, have no placed references or active swap-rule uses.
The default, autumn and winter Falkreath center-tree assets are present.
Missing future/test Beyond Skyrim models are author-library stubs, not proof
of missing playable trees. The shipped BSAssets archive matches its source.

A real BOS snow-cell swap referred to SwordFern06Snow.nif omitted from the
Grumbledook Swordferns optional PBR archive. The repair retains SwordFern06's
geometry and uses the author's snow diffuse, normal and RMAO textures. Native
NIF comparison confirms the same material-only transformation as the author's
SwordFern05Snow; wind, geometry and shader flags are unchanged. The original
source is Nexus mod163949 file685316. Do not upload the derived source mesh
without permission; reconstruct it from that archive for the installer.

Bruma requires special output priority. Bruma - All Fixes for Custom LODs -
Non-Seasons (Nexus143795) must overwrite all terrain, TexGen and DynDOLOD output.
Generate BSHeartland with Ultra tree LOD and CreateEmptyBTT=1 to preserve distant
Cyrodiil's supplied standard tree LOD. Remove only BSHeartland's generated
Occlusion.esp override following the author's culling workaround. Other worlds
retain their generated occlusion. Child worlds using parent LOD inherit their
parent output; test/editor worlds without LOD definitions are not generation
candidates. Final generator coverage and gameplay checks remain pending.

References: https://dyndolod.info/Mods/Beyond-Skyrim-Bruma and
https://www.nexusmods.com/skyrimspecialedition/mods/143795 .


Forest Fragments 3.0 uses the author Plants and Debris main file and matching Merged Falkreath patch. Both source files match archive hashes. This update removes the two invalid Dragonborn snow-tree STAT overrides, restoring WardenWood meshes at the original model paths. Its plugin and selected patch contain no LAND records, so the completed terrain output remains applicable. PG and TexGen are regenerated after the update.

Floral grass missing separate normal textures are documented unused placeholders in the author FAQ. TexGen uses its supported flat-normal fallback. The full grass meshes and diffuse textures are retained; grass LOD is generated with HD Grass 0/100/0 and CS optimized grass assets. Runtime appearance validation remains pending.


DynDOLOD NG preflight requires four official plugins to be cleaned: Update.esm, Dawnguard.esm, HearthFires.esm and ccvsvsse004-beafarmer.esl. Use xEdit 4.1.5f Quick Auto Clean through MO2, one target plus its masters at a time. Separate copies are placed in FROST - Cleaned Official Plugins; the original winning files are backed up and retained. The four deleted large references reported before cleaning are Update:000C8701, Dawnguard:000E1F71, HearthFires:000E8D9D and Fishing:000FA38B. Native Quick Auto Clean completed for all four plugins. The four deleted large references are restored with native Undelete and Disable; original sources remain unchanged. The 21 removed ITM LAND overrides inherit semantically identical terrain from their masters after ignoring unused padding, so the terrain build remains applicable. Existing deleted navmeshes and unmatched Creation Club placeholder references were retained by native cleaning; no navigation was fabricated. Reconstruct official plugin changes from owned game sources through Wabbajack; do not inline or host Bethesda masters.


Obscure's College of Winterhold contains a malformed cwhcm_setchangeonquestprog_03.pex: its bytes are a compiler log rather than executable Papyrus. The published script fix (Nexus62720 file260213, version1.0) supplies a valid PEX with magic FA57C0DE and is installed after the College source. The source BSA remains untouched; the repair changes no terrain, meshes or TexGen inputs. DynDOLOD was cancelled normally before installing it, and the final pass is restarted from the saved all-world preset.


The diagnostic DynDOLOD tree report selects the repaired Warden ash02 and dead-snow02 checksum resources. The canonical dead-snow04 alias is not selected because the active plugin uses Ulvenwald's distinct letreepineforestdeadsnow04 model instead. Its matching new HD billboard is retained; the canonical Warden geometry is not forced onto that different model.

The diagnostic pass exposed six Bruma CELLs assigned to Skyrim's AlexCoast02 region. The native compatibility patch removes only those invalid region assignments and preserves the winning Northern Roads world bounds. It adds no LAND, navigation or placed-object records. A second repair removes one empty, unreferenced RYFTEN Windows CELL at Riften grid 0,-1; the Medieval Markets CELL and its table remain intact. Native checks and a record-by-record comparison pass.

Seven additional plugins were cleaned with native Quick Auto Clean on separate copies: the Capital Windhelm Embers patch, COTN Falkreath Smelter, Umbra, Goldbrand, Riverwood eFPS patch, Across the Border Bruma patch and Ghosu Auriel. Native cleaning restores 26 deleted references and removes one identical weapon override. The cleaned copies contain no remaining deleted references; no LAND records change or disappear. Original author plugins remain unchanged.

Ultimate Optimized Scripts Compilation is updated from 1.3 to 1.83 using the author's USSEP AE and runtime 1130+ ObjectReference choices. All 507 deployed files match the selected author source files. The winning Blackreach elevator script now contains the USSEP message property missing from the older compilation. These script and region repairs do not change material, terrain or billboard inputs; DynDOLOD is rerun against them.

Sources: [UOSC](https://www.nexusmods.com/skyrimspecialedition/mods/122999), [ignored-cell diagnosis](https://dyndolod.info/Messages/Ignoring-Cell).


Material reconstruction: 318 DDS files were moved byte-for-byte into 43 source-specific output groups after the main material output. Each group points Wabbajack matchAll at its original source archive, including official Creation Club sources. Keep these groups together and preserve their priority. The files are reconstructed during installation rather than redistributed as a mesh/texture bundle. Six overridden General Carius PG meshes were archived; final BodySlide winners remain unchanged.
