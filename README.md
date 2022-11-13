![Sonic Frontiers Mod Hub Logo](Logo-temp.png?raw=true)

- This repo will be used for hosting mods, providing convenient links to modding tools and guides on modding Sonic Frontiers. 
- Join the [Hedgehog Engine Modding Discord](https://dc.railgun.works/hems).

# Tools
- [HedgeArcPack](https://github.com/CamoRF/Sonic-Frontiers-Mod-Hub/raw/main/tools/HedgeArcPack_WIP_Frontiers.7z) : unpack/pack ".pac" file format
- [SkythTools](https://github.com/blueskythlikesclouds/SkythTools) : A collection of tools for modern Sonic the Hedgehog games 
- [HedgeLib](https://github.com/Radfordhound/HedgeLib) : A C# library and collection of tools that aims to make modding games in the Sonic the Hedgehog franchise easier. 
- [HedgeNeedle](https://github.com/CamoRF/Sonic-Frontiers-Mod-Hub/raw/main/tools/HedgeNeedle.7z) : Placeholder
- [Hedgehog Engine 2 Mesh Blender Importer](https://github.com/Turk645/Hedgehog-Engine-2-Mesh-Blender-Importer) : Plugin for importing the games models in Blender
- [Eternity Audio Tool](https://animegamemods.freeforums.net/thread/618/eternity-audio-tool-link-tutorial) : Used for ripping audio from the game
- [ModelFixerPost2020](https://github.com/CamoRF/Sonic-Frontiers-Mod-Hub/raw/main/tools/ModelFixerPost2020.zip) : Can possibly fix broken models

# Mods

- [Releases](https://github.com/CamoRF/Sonic-Frontiers-Mod-Hub/releases)

# File Structure

- SonicFrontiers\image\x64\raw\
  - \bmpfont\ : empty
  - \boss\ : boss textures, materials, models, levels and animations
  - \character\ : character textures models, materials and animations
  - \decotext\ : unknown
  - \dlc\ : additional content
  - \enemy\ : boss textures, materials, models and levels and animations
  - \event\ : real-time cutscenes/events? 
  - \gedit\ : setdata/object layout
  - \general\ : unknown
  - \hedgehog\ : engine related level, debug, sound and fonts; mostly empty
  - \miniboss\ : mini boss textures, materials, models, levels and animations
  - \misc\ : miscellaneous textures and levels; needs to be looked into more
  - \movie\ : non real-time custscenes
  - \navmesh\ : NPC navigation path meshes
  - \scalablefont\ : fonts
  - \script\ : various scripts and functions, .lua format is common
  - \sound\ : sounds and music
  - \stage\ : world/level textures, materials, models and LODs; most of the games textures can be found here
  - \text\ : subtitles, skills and other text popups
  - \texture_streaming\ : unknown, most likely engine related files for streaming in textures
  - \ui\ : user interface textures
  
# File Formats

- Placeholder

# Guides

# Model Import Tutorial Video (credits to junior#0001)

[Sonic Frontiers Modding - Model Import Tutorial](https://youtu.be/B_-YJ2I1_M4)

FAQ
- Q: How do I import the .model into blender? 
  - A: Google "How to install a blender add-on and follow the tutorial", here's the [plugin](https://cdn.discordapp.com/attachments/987489054377508924/1041430235809316934/Hedgehog-Engine-2-Mesh-Blender-Importer-main.zip) if you missed it. 
- Q: ALT+R isn't working, why?
  - A: Turn off hotkeys/keybindings for AMD or NVIDIA overlays
- Q: My model is invisible, why?
  - A: Make sure your materials all have proper names. Don't leave them as the default. 


# Model Ripping (credits to stix#1997)

1. First off, you're gonna want to extract the .pac files using [HedgeArcPack](https://cdn.discordapp.com/attachments/987489054377508924/1039653178494431272/HedgeArcPack_WIP_Frontiers.7z)

2. Depending on what pac file you extract there may be no textures, inorder to fix this, use [SkythTools](https://github.com/blueskythlikesclouds/SkythTools) NeedleTextureStreamingPackage

3. Some .model files may need to be extracted using [HedgeNeedle](https://cdn.discordapp.com/attachments/464963211410669579/1039655306378100816/HedgeNeedle.7z)

4. Import the model using [Hedgehog Engine 2 Mesh Blender Importer] (https://github.com/Turk645/Hedgehog-Engine-2-Mesh-Blender-Importer). Extract the zip and install the py files instead of installing the zip.

5. Make sure after using Hedgeneedle, you copy the skl.pxd into the folder of the extracted models and rename the model to the same name as the skeleton except for extension, leave the skl.pxd files name the same

# Maps Required For Textures

- Abd = Albedo/Base Color Map
- Nrm = Normal Map
- Fal = Fresnel Color Map
- CDR = Subsurface Scattering Color basically
- Ems = Emission 
- PRM_R = Reflectivity (Specular F0)
- PRM_G = Smoothness 
- PRM_B = Metalness 
- PRM_A = Ambient Occlusion

# Audio Ripping (credits to ✨Kat✨#1234)

Tools needed
- Sonic Audio Tools on Skyth's [Github](https://github.com/blueskythlikesclouds/SkythTools)
- [Eternity Audio Tool](https://animegamemods.freeforums.net/thread/618/eternity-audio-tool-link-tutorial)
- [Foobar](https://www.foobar2000.org/download)
- [VGMStream](https://discord.com/channels/945689739447664640/987489054377508924/1041368205077254144)

1. Go to the .acb which you wish to extract (In this case for BGM you'll want to go into sound folder and find bgm.acb), drag and drop the .acb file onto AcbEditor.exe in Sonic Audio Tools and after a while you'll get a folder in the sound folder named after the .acb you just extracted, open it and you will see all of the audio files in .hca form.

2. To playback these tracks you will need Foobar2000 with VGMStream, install Foobar2000 and click on VGMStream and apply it. Then go to the main menu of Foobar2000, go to file and click open, press CTRL+A on the folder with all of the files you want to listen to and play them all back. If you wish to extract the audio, right click it, go to convert and quick convert, I recommend converting to either .wav or .ogg.

3. To edit the tracks, make sure you copy both of the extracted folder .acb and the original .acb to a different folder. Listen to the audio track you wish to use and use Foobar2000 to listen to the audio tracks in that folder, once you have the name of a track you wish to replace. Make a sound file (.wav/.ogg) you wish to replace that track with, open Eternity's Audio Tool 1.0b, click File and Convert to .hca, select the audio file you want to change into a .hca and rename it to the audio file you want to change inside of the extracted .acb folder. Then replace the track and drag and drop the extracted folder .acb onto AcbEditor.exe. You've now changed audio in Sonic Frontiers, you can do the rest. 

# Project Resaerch

- INCREASED DRAW DISTANCE
  - Possible strings in hex editor related to LOD in SonicFrontiers.exe :
    - distanceScale
    - distanceDecayEnabled
    - u_grass_lod_distance
    - u_grass_dither_distance
    - lodDistances
    - grassDitherStart
    - graassDitherEnd
