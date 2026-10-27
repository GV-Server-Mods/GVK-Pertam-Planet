# GVK_Pertam_Planet

Kharak, the planet for the GV: Deserts of Kharak (GVK) Space Engineers server. It is based on vanilla Pertam, with smooth roads, higher peaks, canyons you can drive through, custom voxel materials, Kharak weather and the Xylanthia skybox.

Published as [Workshop 3051204767](https://steamcommunity.com/sharedfiles/filedetails/?id=3051204767).

## Philosophy
- **A planet made for rovers.** Smooth roads, passes and drivable canyons, so driving is the way to travel.
- **Kharak weather is part of the rules.** Hazard values for storms and radiation sit in the weather definitions, not in a script.

## Requirements
Loaded with the rest of the server mods ([Steam collection](https://steamcommunity.com/sharedfiles/filedetails/?id=2650582206)). Zone and spawn rules are in GVK-Derelicts and GVK_Settings, not here.

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

## Quick links
- Hub board and issues: [GV-Server-Mods/GVK-Settings](https://github.com/GV-Server-Mods/GVK-Settings)
- Steam guide: [players' rules and gameplay](https://steamcommunity.com/sharedfiles/filedetails/?id=2781522559); mod collection: [2650582206](https://steamcommunity.com/sharedfiles/filedetails/?id=2650582206)
- Skills: [se-dev-kharak](https://github.com/GV-Server-Mods/se-dev-kharak)

## Build

Open the folder in VS Code and press **Ctrl+Shift+B**. MDK2 (`Mal.Mdk2.ModPackager`) builds the project and deploys the mod to `%APPDATA%\SpaceEngineers\Mods\GVK_Pertam_Planet`. Add that local mod to a test world to try changes before uploading.

## Credits

The Xylanthia skybox is used with permission from SixDice (Sixie), granted before he passed away in 2021. See `SixDice skybox note.txt`.

## Issues

Tracked in the GVK hub: [GV-Server-Mods/GVK-Settings](https://github.com/GV-Server-Mods/GVK-Settings/issues).

## License

[MIT](LICENSE.txt). The Xylanthia skybox is SixDice's work, used with permission, and is not covered by this license.
