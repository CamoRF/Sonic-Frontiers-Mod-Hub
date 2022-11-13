# Sonic Frontiers Mod Hub
- This repo will be used for both hosting mods, providing convientant links to modding tools and guides on modding Sonic Frontiers. 

# Tools (placeholder)
- [HedgeArcPack](https://cdn.discordapp.com/attachments/987489054377508924/1039653178494431272/HedgeArcPack_WIP_Frontiers.7z)
- [SkythTools](https://github.com/blueskythlikesclouds/SkythTools)
- [HedgeNeedle](https://cdn.discordapp.com/attachments/464963211410669579/1039655306378100816/HedgeNeedle.7z)
- [Hedgehog Engine 2 Mesh Blender Importer] (https://github.com/Turk645/Hedgehog-Engine-2-Mesh-Blender-Importer)
- [Eternity Audio Tool] (https://animegamemods.freeforums.net/thread/618/eternity-audio-tool-link-tutorial)

# Guides (placeholder)

Abd = Albedo/Base Color Map
Nrm = Normal Map
Fal = Fresnel Color Map
CDR = Subsurface Scattering Color basically
Ems = Emission 
PRM_R = Reflectivity (Specular F0)
PRM_G = Smoothness 
PRM_B = Metalness 
PRM_A = Ambient Occlusion

- Model Ripping (credits to stix#1997)

1. First off, you're gonna want to extract the .pac files using [HedgeArcPack](https://cdn.discordapp.com/attachments/987489054377508924/1039653178494431272/HedgeArcPack_WIP_Frontiers.7z)

2. Depending on what pac file you extract there may be no textures, inorder to fix this, use [SkythTools](https://github.com/blueskythlikesclouds/SkythTools) NeedleTextureStreamingPackage

3. Some .model files may need to be extracted using [HedgeNeedle](https://cdn.discordapp.com/attachments/464963211410669579/1039655306378100816/HedgeNeedle.7z)

4. Import the model using [Hedgehog Engine 2 Mesh Blender Importer] (https://github.com/Turk645/Hedgehog-Engine-2-Mesh-Blender-Importer). Extract the zip and install the py files instead of installing the zip.

5. Make sure after using Hedgeneedle, you copy the skl.pxd into the folder of the extracted models and rename the model to the same name as the skeleton except for extension, leave the skl.pxd files name the same

# Mods (placeholder)

- [Releases](https://github.com/CamoRF/Sonic-Frontiers-Mod-Hub/releases)

# Projects

- Possible strings in hex editor related to LOD:

Search for these strings in the .exe:

distanceScale
distanceDecayEnabled
u_grass_lod_distance
u_grass_dither_distance
lodDistances
grassDitherStart
graassDitherEnd
