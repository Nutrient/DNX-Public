<div align="center">

<img src="docs/images/dnx_title.png" alt="DNX" width="420">

**An in-game overlay mod for Dragon Nest: quality of life, graphics, a damage meter and more.**

[![Latest release](https://img.shields.io/github/v/release/Nutrient/DNX-Public?label=release&color=1e90ff)](../../releases/latest) [![Downloads](https://img.shields.io/github/downloads/Nutrient/DNX-Public/total?color=1e90ff)](../../releases) [![Discord](https://img.shields.io/badge/Discord-join-5865F2?logo=discord&logoColor=white)](https://discord.gg/jEcFtkX5N6) [![Buy me a coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee-support-FFDD00?logo=buymeacoffee&logoColor=black)](https://buymeacoffee.com/nutrient)

[Download](../../releases/latest) · [Install](#install) · [Features](#features) · [Troubleshooting](#troubleshooting) · [Discord](https://discord.gg/jEcFtkX5N6)

</div>

---

DNX adds an in-game overlay to Dragon Nest with quality-of-life and graphics options, a damage meter, chat
filters, automation helpers and a quick-login helper. It starts through its own launcher and does not modify the
game files.

- **Clients:** North America and Southeast Asia
- **Open the overlay:** press `/` in game
- **Updates:** the launcher updates itself, the mod and its data on every start

## Install

1. Download the latest `DNXv<version>.zip` from [Releases](../../releases/latest).
2. Extract the `dnx` folder to any location, for example `C:\dnx`. Do not put it in the game folder.
3. Make sure the game is up to date. If a patch came out, start the game once with the official launcher.
4. Run `dnx_launcher.exe`. On first start, pick your server and the Dragon Nest folder (the folder with
   `DragonNest_x64.exe`).
5. In game, press `/` to open the overlay.

### "Windows protected your PC" / antivirus warnings

DNX is a small, unsigned hobby project, and the launcher loads the mod into the game process. Browsers, Windows
SmartScreen and antivirus programs can warn about or block `dnx_launcher.exe` or `dnx_mod.dll`. This is a false
positive.

> [!IMPORTANT]
> Only do the steps below for a copy you downloaded from this repo's [Releases](../../releases) page.

**Browser** ("isn't commonly downloaded"): open the download list and choose Keep (Edge: `...` > Keep > Show more >
Keep anyway; Chrome: Keep / Download dangerous file).

**SmartScreen** ("Windows protected your PC"): click "More info", then "Run anyway".

![SmartScreen: More info, then Run anyway](docs/images/smartscreen_run_anyway.jpg)

**Microsoft Defender:** add `dnx_launcher.exe` as an exclusion so Defender stops blocking it.

1. Open Windows Security > Virus & threat protection.
2. Under "Virus & threat protection settings", click "Manage settings".
3. Under "Exclusions", click "Add or remove exclusions".
4. Click "Add an exclusion" > File, and pick `dnx_launcher.exe` in your `dnx` folder.

![Defender exclusion for dnx_launcher.exe](docs/images/defender_exclusion.png)

If Defender already removed a file, restore it first: Windows Security > Virus & threat protection > Protection
history > the entry > Actions > Allow / Restore. For another antivirus, add the same exclusion in its settings.

## Features

The overlay groups settings into the categories below. Settings that are less stable have an amber background and
a warning sign; they are off by default.

### Gameplay

| Feature | What it does |
|---|---|
| Fast looting | Faster pickup, including stages where you pick up items without a pet |
| Shorter pet leash | Keeps your pet closer to you |
| No double-tap tumble | Turns off double-tap tumble; use Shift+direction instead |
| Skips | Auto-skip cutscenes, the intro video, the Board Game animation and the Collapsed Dimensional Rift portal animation |
| Instant craft | Crafting at the blacksmith finishes at once |
| Hide Beginner Guide | Removes the Beginner Guide window |

### Camera

| Feature | What it does |
|---|---|
| Zoom and view | Zoom limits, field of view (30 to 100 degrees) with Keep horizon, tilt limit |
| Free camera | Press a key to fly the camera away from your character, with adjustable fly and turn speed |
| Camera effects | Camera shake, radial blur (Stock / Reduced / Off), skill camera movement, skill motion blur |

### Graphics

| Feature | What it does |
|---|---|
| Shader quality | Stock, Optimized or Low |
| Resolution | Render scale from 50% to 200% (supersampling above 100%, AMD FSR 1 below), sharpening, 4x / 8x / 16x texture filtering |
| Anti-aliasing and bloom | SMAA or sharper FXAA, Dual Kawase bloom with strength and quality |
| Shadows | Shadow distance, skip small distant shadows |
| View distance | How far the world is drawn |

### Visual style

| Feature | What it does |
|---|---|
| Color LUTs | Built-in looks, your own LUT files, and Protanopia, Deuteranopia and Tritanopia colorblind modes |
| Scene effects | Color style presets, ambient occlusion, bokeh depth of field, film grain, chromatic aberration, vignette, deband |
| Fog and outlines | Adds fog and outlines to the scene |
| Character style | Anime or Adventure look, with cel strength, rim side and flat lit band |

### Effects

| Feature | What it does |
|---|---|
| Skill-effect opacity | Fade skill effects, separately for you and for other players |
| Particles | Particle density, hide particles by type, keep drop effects for good items |
| Pets | Hide your own or other players' pets |

### Performance

| Feature | What it does |
|---|---|
| Frame rate | Frame rate cap, lower FPS in the background, frame latency |
| CPU savings | Faster table lookups, faster head names, batch interface drawing, skip allocation bookkeeping |
| Loading and memory | Faster startup (skips the animation-file check when nothing changed), texture cache, lower memory use |

### Chat

| Feature | What it does |
|---|---|
| Chat window | Hide the chat window, set its width |
| Messages | Profanity filter, timestamps with date and time format, damage contribution messages |
| Courier birds | Hide Blue / Red Courier Bird messages, or block them from specific senders |
| System tab | System messages only in the System tab, with exception presets and your own patterns |
| Loot messages | Filters for solo and party play, by grade or by item list |

### Damage meter and HUD

| Feature | What it does |
|---|---|
| Damage meter | Boss / Dungeon, Nest and DPS chart tabs, several styles, wide or compact panel, movable position, show/hide key |
| DPS chart | 5s rolling DPS, 1s DPS, average DPS and party total, with a choice of players on the chart |
| Damage numbers | Shown as their type (CRIT, BURN, POISON, ...) |
| FPS / ping | Readout in the game's own text, visible with the overlay closed |
| Countdown / stopwatch | Timer widget |
| Portrait | Static class icon in place of the animated face |
| Stream view | A second "DNX Stream View" window without the overlay, damage meter or timer, for OBS Window Capture or Discord window share |

### Automation

| Feature | What it does |
|---|---|
| Follow | Follow a party leader or member, with live status, tracking and distance |
| Selection Pouch opener | Pick a pouch and reward, set how many to open (bag and cash inventory) |
| Skill Jade unseal | Auto-unseals sealed +0 jades |

### Quick Login

| Feature | What it does |
|---|---|
| Saved accounts | Fill in the login boxes with one click on the login screen; saved logins are shared by every client |

> [!WARNING]
> In windowed mode the automatic 2nd-password step is flaky and can crash the game; play fullscreen or untick
> "Auto-continue past login". Saved logins are scrambled, not strongly encrypted; do not save accounts on a shared
> computer.

### Launcher

| Feature | What it does |
|---|---|
| Setup window | Pick the server (North America / Southeast Asia) and install folder; hold Shift at start to reopen it |
| Version check | Checks that the game is up to date before launching |
| Auto-update | Updates itself, the mod and its data on every start; turn off or pin a release in Help & About > Updates, or start with `--no-update` |
| Multiple clients | No setup needed: each client gets its own configuration and a numbered window title (`DragonNest - i0`, `DragonNest - i1`, ...) |
| One config file | All settings in `config.json` next to the launcher |

### Help & About

| Feature | What it does |
|---|---|
| Overlay key | Rebind the key that opens the overlay |
| Hook status | Shows which game hooks are active |
| Performance recording | Records data for stutter / FPS bug reports |
| Updates | Auto-update on/off and target version |
| Community | Discord and Support development links |

## Reporting a bug

Report bugs on [Discord](https://discord.gg/jEcFtkX5N6) or in [Issues](../../issues). Logs are in the `dnx` folder:

- `logs\session\` holds one log per launch, named by date and time. Attach the newest one.
- `logs\crash\` holds a crash report if the game crashed, or a freeze report if it hung for 10 seconds or more.
  Attach it too if there is one.

Describe what you did and what went wrong. For stutter or FPS problems, use Performance recording on the Help &
About page.

> [!CAUTION]
> Logs from versions before v0.8.2 can reveal a saved 2nd password. Before you share an old log, delete the lines
> that contain `login_hook: PIN`.

## Troubleshooting

| Problem | Fix |
|---|---|
| "Your game client is out of date" | Update the game with the official launcher, then run `dnx_launcher.exe` again. |
| Launcher does nothing | Hold Shift while starting it and check that the install folder is the folder with `DragonNest_x64.exe`. |
| No overlay in game | Press `/` and check the hook status on Help & About. |
| Reset all settings | Close the game and delete `config.json`. Saved logins in `dnx_login.dat` are kept. |

## Uninstall

Delete the `dnx` folder. The game files were not changed, and the game keeps working with the official launcher.

## Support

DNX is a free hobby project. If you like it, you can [buy me a coffee](https://buymeacoffee.com/nutrient) or join
the [Discord](https://discord.gg/jEcFtkX5N6).

## Disclaimer

DNX is an unofficial fan project. It is not affiliated with or endorsed by the publishers of Dragon Nest. Using
third-party tools can break the game's terms of service; use DNX at your own risk.
