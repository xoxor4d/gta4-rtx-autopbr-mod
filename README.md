## AutoPBR Remix-Mod for the GTAIV RTX Remix Compatibility Mod

This is an actual __remix__ mod for GTAIV. It is meant as a base for the [GTAIV RTX Remix Compatibility Mod](https://github.com/xoxor4d/gta4-rtx).  

<br>

A [custom build of the remix runtime ](https://github.com/xoxor4d/dxvk-remix/tree/feat/AutoPBR) was used to dump textures at runtime whenever
they were used for rendering. The compatibility mod provided additional information about each texture via the remixApi.
Texture associations were build and a usda with overwrites was generated. Additional processing on the dumped textures was done 
to convert dx9 normalmaps to remix compatible normalmaps and specularmaps were converted to roughness maps via python scripts.

<br>

##  Credits
- [NVIDIA - RTX Remix](https://github.com/NVIDIAGameWorks/rtx-remix)
- [People of the showcase discord](https://discord.gg/j6sh7JD3v9) - especially the nvidia engineers ✌️
- [danlopand](https://github.com/DANLOPAND) - multiple PR's 👍
- All 🍓 Testers

<br>

### Installation

Use the installer that comes with the Compatibility Mod _OR_ install manually:
- [Download repo as zip](https://github.com/xoxor4d/gta4-rtx-autopbr-mod/archive/refs/heads/master.zip)
- Place the `z_gta4rtx_autopbr` folder into the `rtx-remix\mods\` folder found in the GTAIV root folder  
(see Folder Structure below)

<br>

<div align="center" markdown="1">

<h2>Folder Structure</h3>
<a name=""></a>
</div>

```
.  
├─ ...
├─ 📁 steamapps
│  └─📁 common
│     └─📁 Grand Theft Auto IV
│       └─📁 GTAIV
│         ├── 📜 GTAIV.exe.exe
│         ├── 📜 d3d9.dll
│         ├── 📜 ...
│         │
│         ├── 📁 .trex
│         │   ├── 📜 d3d9.dll
│         │   ├── 📜 NvRemixBridge.exe
│         │   └── ...
│         │
│         ├── 📁 rtx_comp
│         └── 📁 rtx-remix
│             └─📁 mods
│               └─📁 z_gta4rtx_autopbr
│                 ├── 📜 comp_autoconvert.usda
│                 ├── 📜 mod.usda
│                 └── ...
└── ...  
```
