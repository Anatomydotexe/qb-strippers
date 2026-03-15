# qb-strippers

A QBCore resource that spawns animated stripper NPCs inside the **Gabz Vanilla Unicorn MLO** for FiveM. Fully compatible with the latest QBCore framework and FiveM standards.

## Features

- Animated stripper NPCs with native GTA V dance/lap dance animations
- Supports pole dances, private dances, and lap dances (dual NPC)
- Positions tuned specifically for the Gabz Vanilla Unicorn MLO layout
- Lightweight — client-side NPC spawning with no unnecessary server load
- Easy configuration via `config.lua`

## Requirements

- [QBCore Framework](https://github.com/qbcore-framework/qb-core)
- [Gabz Vanilla Unicorn MLO](https://gabzinteriors.com) (or compatible interior)

## Installation

1. Download or clone this repository into your server's `resources` folder:
   ```
   resources/[qb]/qb-strippers
   ```
2. Add the following to your `server.cfg`:
   ```
   ensure qb-strippers
   ```
3. Restart your server or use `refresh` + `ensure qb-strippers` in the console.

## Configuration

Edit `config.lua` to adjust NPC positions, models, and animations:

```lua
Config.Stripper = {
    { x = 109.05, y = -1283.27, z = 27.75, heading = 212.67, model = "a_f_y_topless_01", dict = "...", anims = { "..." } },
    -- add or remove entries as needed
}
```

Each entry supports:
| Key | Description |
|---|---|
| `x, y, z` | World position of the NPC |
| `heading` | Direction the NPC faces |
| `model` | Ped model to use |
| `dict` | Animation dictionary |
| `anims` | List of animation clips to play |

## License

MIT — free to use and modify. Credit appreciated but not required.
