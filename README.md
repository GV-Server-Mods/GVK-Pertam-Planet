# GVK_Pertam_Planet

Kharak, the planet for the GV: Deserts of Kharak (GVK) Space Engineers server. It is based on vanilla Pertam, with smooth roads, higher peaks, canyons you can drive through, custom voxel materials, Kharak weather and the Xylanthia skybox.

Published as [Workshop 3051204767](https://steamcommunity.com/sharedfiles/filedetails/?id=3051204767).

## Contents

| File | What it defines |
|---|---|
| `Content/Data/PertamKharak.sbc` | The `PertamKharak` planet generator: terrain, ores, materials, weather generator |
| `Content/Data/PlanetDataFiles/PertamKharak/` | Heightmaps and material maps |
| `Content/Data/WeatherEffects_Jakaria.sbc` | Kharak versions of vanilla weathers (sandstorms, rain, fog, ...) with GVK hazard values |
| `Content/Data/WeatherEffects_AlphaKharak.sbc` | Kharak-only weathers (`RadiationStorm`, `KharakClear`, `BlueSky`) and a milder `Hailstorm` |
| `Content/Data/Environment.sbc` | Replaces the vanilla `Default` environment: skybox, sun, lighting, eye adaptation, ship speed and rotation caps |
| `Content/Data/VoxelMaterials_planetary_AlphaKharak.sbc` | Road and sand voxel materials |
| `Content/Textures/`, `Content/Audio/` | Skybox, road texture, radiation storm sound |

`Environment.sbc` replaces the whole vanilla environment definition, so any section it leaves out falls back to the game's code defaults, not to Keen's `Environment.sbc`.

## Build

Open the folder in VS Code and press **Ctrl+Shift+B**. MDK2 (`Mal.Mdk2.ModPackager`) builds the project and deploys the mod to `%APPDATA%\SpaceEngineers\Mods\GVK_Pertam_Planet`. Add that local mod to a test world to try changes before uploading.

## Credits

The Xylanthia skybox is used with permission from SixDice (Sixie), granted before he passed away in 2021. See `SixDice skybox note.txt`.

## Issues

Tracked in the GVK hub: [GV-Server-Mods/GVK-Settings](https://github.com/GV-Server-Mods/GVK-Settings/issues).

## License

[MIT](LICENSE.txt). The Xylanthia skybox is SixDice's work, used with permission, and is not covered by this license.
