# DNX-Public

Public repo for DNX Dragon Nest Mod.

DNX adds an in-game overlay to Dragon Nest with quality-of-life and graphics options, a damage meter,
party follow and a quick-login helper. It starts through its own launcher; the game files are not modified.
Download the latest `DNXv<version>.zip` from [Releases](../../releases), extract the `dnx` folder anywhere
(not inside the game folder) and run `dnx_launcher.exe`. Press `/` in game to open the overlay.

## Features

### Quality of life
- Fast looting
- Camera zoom limits and camera-shake toggle
- Shorter pet leash
- Auto-skip cutscenes
- Instant craft at the blacksmith
- Skip the Board Game animation
- Hide the Beginner Guide
- Damage numbers shown as their type (CRIT, BURN, POISON, ...)

### Graphics
- Shader quality: Stock, Optimized or Low
- View distance
- Frame rate cap
- Stream view: a second "DNX Stream View" window that shows the game without the overlay, damage meter or
  timer, for OBS Window Capture or Discord window share

### HUD
- Damage meter with Boss / Dungeon, Nest and DPS chart tabs, several styles, compact mode, movable position
  and a show/hide key
- Countdown / stopwatch widget

### Automation
- Follow a party leader or member

### Login
- Quick Login: save accounts and fill in the login boxes with one click on the login screen.
  In windowed mode the automatic 2nd-password step is flaky and can crash the game; play fullscreen or
  untick "Auto-continue past login". Saved logins are scrambled, not strongly encrypted.

### Launcher
- Setup window for server (North America / Southeast Asia) and install folder; hold Shift at start to
  reopen it
- Checks the game is up to date before launching
- Updates itself (launcher, mod and data) from the latest release on every start; turn off with
  `--no-update` or `"launcher": {"update": {"enabled": false}}` in `config.json`
- All settings in one `config.json` next to the launcher

### Help & support
- Rebindable overlay key
- Hook status page
- Performance recording for stutter / FPS bug reports

## Disclaimer

DNX is an unofficial fan project, not affiliated with or endorsed by the publishers of Dragon Nest.
Using third-party tools may break the game's terms of service; use it at your own risk.
