# BetterArch

<p align="center">
<img width="300" alt="BetterArch Logo" src="https://github.com/user-attachments/assets/9eb01b7b-3eda-43c4-99d4-816b62276753" />
</p>

<p align="center">
  A modern emulator frontend for the Nintendo Switch.
  <br>
  Multiple systems, beautiful themes, and easy save states.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-0.4.0-8F7CFF" alt="Version">
  <img src="https://img.shields.io/badge/platform-Nintendo%20Switch-E60012" alt="Platform">
  <img src="https://img.shields.io/badge/status-Early%20Access-47E3D1" alt="Status">
</p>

<p align="center">
  <a href="../../releases/latest"><b>Download BetterArch</b></a>
</p>

---

## Screenshots

<p align="center">
  <img width="800" alt="RetroGlass Theme" src="https://github.com/user-attachments/assets/e63d05ef-6eee-4f39-9161-44ae3be00e99" />
  <img width="800" alt="Retro Theme" src="https://github.com/user-attachments/assets/dca83fe8-e391-44f7-ab72-0eacf7f8ebef" />
</p>

## Features

- 🎮 **Multiple systems** — Play games from several classic consoles.
- ✨ **Two themes** — Modern RetroGlass and classic Retro.
- 💾 **Save states** — Save and resume games wherever you want.
- 🕹️ **Simple controls** — Automatic controller mapping.
- ⚡ **BetterMelon** — A customised Nintendo DS emulator.
- 🔄 **Multiple emulators** — Switch emulators for individual games.
- 🖼️ **Automatic artwork** — Download cover art and display proper game names.
- ⌨️ **Custom hotkeys** — Configure shortcuts and access the in-game menu.

## Supported Systems

| System | Default Emulator |
|---|---|
| NES | FCEUmm |
| SNES | Snes9x |
| Nintendo 64 | Mupen64Plus-Next |
| Game Boy / Color | Gambatte |
| Game Boy Advance | mGBA |
| Nintendo DS | BetterMelon |
| PlayStation 1 | PCSX ReARMed |

Alternative emulators are available for selected systems.

## Requirements

- Nintendo Switch running Atmosphère custom firmware.
- Homebrew Menu.
- Approximately 130 MB of free SD card space.
- Your own legally obtained game backups.
- Your own BIOS and firmware dumps for Nintendo DS games.

## Installation

1. Download the latest release from the [Releases page](../../releases/latest).
2. Extract the ZIP file.
3. Copy the `switch` and `BetterArch` folders to the root of your SD card.
4. Place your games in the appropriate folders below.
5. Hold **R** while launching a game to open the Homebrew Menu.
6. Launch **BetterArch**.

any issues please contact me on  **Discord:** [Better](https://discord.gg/q4qknMESsr)

### Game folders

| System | Folder | File types |
|---|---|---|
| NES | `BetterArch/roms/nes/` | `.nes`, `.fds` |
| SNES | `BetterArch/roms/snes/` | `.sfc`, `.smc` |
| N64 | `BetterArch/roms/n64/` | `.z64`, `.n64`, `.v64` |
| Game Boy | `BetterArch/roms/gb/` | `.gb` |
| Game Boy Color | `BetterArch/roms/gbc/` | `.gbc` |
| Game Boy Advance | `BetterArch/roms/gba/` | `.gba` |
| Nintendo DS | `BetterArch/roms/nds/` | `.nds` |
| PlayStation 1 | `BetterArch/roms/psx/` | `.cue` / `.bin`, `.chd`, `.pbp` |

Extract compressed games before adding them.

**Important:** Launch BetterArch through the Homebrew Menu, not the Album. The Album provides limited memory and may cause games to fail.

### Nintendo DS BIOS

Place your own BIOS and firmware files in `BetterArch/system/`:

- `bios7.bin` — 16 KB
- `bios9.bin` — 4 KB
- `firmware.bin` — 256 KB

## Controls

| Button | Action |
|---|---|
| A | Launch game |
| ZR / Hold A | Game options |
| X | Favourite game |
| Y | Search |
| + | Settings |
| − | Rescan games |
| B, B | Close BetterArch |
| − and + (in game) | Open game menu |
| − and R (in game) | Save state |
| − and L (in game) | Load state |
| − and X (in game) | Show FPS |

## FAQ

**My game isn't showing up.**

Check that it's in the correct folder, extract it if necessary, and press **−** to rescan.

**My Nintendo DS game won't launch.**

Check that your BIOS and firmware files are present and have the correct sizes.

**My game runs poorly.**

Open its game options with **ZR** and try another available emulator.

**The application crashed.**

Include `runtime.log` and `runtime.prev.log` from `BetterArch/logs/` when reporting the issue.

## Credits

BetterArch uses open-source emulators and libraries, including:

- [melonDS](https://melonds.kuribo64.net/) and [libretro/melonDS](https://github.com/libretro/melonDS)
- [DeSmuME](https://github.com/libretro/desmume)
- [FCEUmm](https://github.com/libretro/libretro-fceumm)
- [Nestopia](https://github.com/libretro/nestopia)
- [Snes9x](https://github.com/libretro/snes9x)
- [Mupen64Plus-Next](https://github.com/libretro/mupen64plus-libretro-nx)
- [Gambatte](https://github.com/libretro/gambatte-libretro)
- [mGBA](https://github.com/libretro/mgba)
- [gpSP](https://github.com/libretro/gpsp)
- [PCSX ReARMed](https://github.com/libretro/pcsx_rearmed)

BetterArch also uses the libretro API, devkitPro, libnx, SDL2, Mesa, and game artwork from [libretro-thumbnails](https://github.com/libretro-thumbnails/libretro-thumbnails) and [GameTDB](https://www.gametdb.com/).

Each project retains its own licence and copyright.

## Source Code

The frontend, runtime, and BetterMelon patches are not yet published in this repository. To request a copy, open an issue.

## Legal

BetterArch does not include or distribute games, BIOS files, or firmware. You must supply your own files.

BetterArch is an independent project and is not affiliated with or endorsed by Nintendo, Sony, Microsoft, or the emulator developers.
