<p align="center">
  
</p>

<h1 align="center">BetterArch</h1>

<p align="center">
  <b>A modern, all-in-one retro emulator frontend for the Nintendo Switch.</b><br>
  Beautiful themes, controls that just work, and save-anywhere on every game.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-0.4.0-8F7CFF" alt="Version 0.4.0">
  <img src="https://img.shields.io/badge/platform-Nintendo%20Switch%20(Atmosph%C3%A8re)-E60012" alt="Platform: Nintendo Switch">
  <img src="https://img.shields.io/badge/status-early%20access-47E3D1" alt="Status: early access">
</p>

<p align="center">
  <a href="../../releases/latest"><b>⬇ Download the latest release</b></a>
</p>

---

## Screenshots

<p align="center">
<img width="1280" height="720" alt="RetroGlass" src="https://github.com/user-attachments/assets/e63d05ef-6eee-4f39-9161-44ae3be00e99" />
<img width="1280" height="720" alt="Retro" src="https://github.com/user-attachments/assets/dca83fe8-e391-44f7-ab72-0eacf7f8ebef" />

## Features

- 🎮 **One app, many systems.** NES, SNES, N64, Game Boy, Game Boy Color, Game Boy Advance,
  Nintendo DS and PlayStation, all from one library.
- ✨ **Two looks.** **RetroGlass**, a modern liquid-glass design, and **Retro**, an old-school
  console menu with CRT scanlines and pixel headings.
- 💾 **Save anywhere.** *Save and exit* remembers exactly where you were, even in games with no
  save points. Ten save-state slots per game.
- 🕹️ **Controls that just work.** Every system is mapped for the Switch automatically. On DS,
  touch the screen to use the stylus.
- ⚡ **BetterMelon.** BetterArch's own Switch-tuned DS emulator (based on melonDS), with JIT, fast
  memory and automatic frameskip.
- 🔁 **Pick the emulator per game.** If a game misbehaves, switch it to another emulator in
  *Game options*.
- 🖼️ **Automatic cover art and real game names.** Box art downloads by itself; messy file names
  like `0434 - game-name (U)` are cleaned up.
- ⌨️ **Hotkeys you can rebind**, plus an in-game menu on **− and +**.

## Supported systems

| System | Default emulator | Alternative |
|---|---|---|
| NES / Famicom | FCEUmm | Nestopia |
| Super Nintendo | Snes9x | Snes9x 2010 |
| Nintendo 64 | Mupen64Plus-Next | — |
| Game Boy / Game Boy Color | Gambatte | mGBA |
| Game Boy Advance | mGBA | gpSP |
| Nintendo DS | **BetterMelon** | DeSmuME |
| PlayStation | PCSX ReARMed | — |

## Requirements

- A Nintendo Switch running **Atmosphère** custom firmware, with the Homebrew Menu working.
- About 130 MB of free SD card space, plus room for your games.
- **Your own** game backups. BetterArch does not include or download any games.
- **For DS games:** your own DS BIOS and firmware dumps (see below).

## Installation

1. Download `BetterArch-v0.4.0.zip` from the [latest release](../../releases/latest) and unzip it.
2. Copy the **`switch`** and **`BetterArch`** folders to the **root** of your SD card.
   If asked, choose *Replace*.
3. Put your games in the matching folder:

   | Folder | File types |
   |---|---|
   | `BetterArch/roms/nes/` | `.nes` `.fds` |
   | `BetterArch/roms/snes/` | `.sfc` `.smc` |
   | `BetterArch/roms/n64/` | `.z64` `.n64` `.v64` |
   | `BetterArch/roms/gb/` | `.gb` |
   | `BetterArch/roms/gbc/` | `.gbc` |
   | `BetterArch/roms/gba/` | `.gba` |
   | `BetterArch/roms/nds/` | `.nds` |
   | `BetterArch/roms/psx/` | `.cue` + `.bin`, `.chd`, `.pbp` |

   Unzip games first; `.zip` / `.7z` files aren't shown.
4. **DS only:** copy your own dumps into `BetterArch/system/`:
   `bios7.bin` (16 KB), `bios9.bin` (4 KB), `firmware.bin` (256 KB).
   DraStic's names (`nds_bios_arm7.bin` …) and its `switch/drastic/system/` folder work too.
5. **Hold R** while opening any installed game to open the Homebrew Menu, then start
   **BetterArch**.

> ⚠️ Don't launch it from the Album. It only gets ~400 MB of memory there, and bigger games
> will fail.

## Controls

| Where | Button | Action |
|---|---|---|
| Home | **A** | Play |
| Home | **ZR** or **hold A** | Game options (emulator, favorite) |
| Home | **X** / **Y** | Favorite / Search |
| Home | **+** / **−** | Settings / Rescan games |
| Home | **B B** | Close BetterArch |
| In game | **− and +** | Menu: Save and exit, states, restart, hotkeys |
| In game | **− and R** / **− and L** | Save state / Load state |
| In game | **− and X** | Show FPS |

## FAQ

**A game is missing from my list.**
Check it's in the right `roms` folder and unzipped, then press **−** to rescan.

**A DS game won't start.**
BetterArch tells you which BIOS file is missing or the wrong size. Add your own dumps to
`BetterArch/system/`.

**A game runs badly or looks wrong.**
Press **ZR** on it and try the other emulator.

**Something crashed.**
Send the files in `BetterArch/logs/` (`runtime.log` and `runtime.prev.log`) when you open an
issue.

## Credits

BetterArch stands on the shoulders of these open-source emulators, used under their own licences:

| Emulator | Project | Licence |
|---|---|---|
| BetterMelon (DS) | Fork of [melonDS](https://melonds.kuribo64.net/) by Arisotura & the melonDS team, via [libretro/melonDS](https://github.com/libretro/melonDS) | GPLv3 |
| DeSmuME (DS) | [libretro/desmume](https://github.com/libretro/desmume) | GPLv2 |
| FCEUmm (NES) | [libretro/libretro-fceumm](https://github.com/libretro/libretro-fceumm) | GPLv2 |
| Nestopia (NES) | [libretro/nestopia](https://github.com/libretro/nestopia) | GPLv2 |
| Snes9x (SNES) | [libretro/snes9x](https://github.com/libretro/snes9x) | Snes9x licence |
| Snes9x 2010 (SNES) | [libretro/snes9x2010](https://github.com/libretro/snes9x2010) | Snes9x licence |
| Mupen64Plus-Next (N64) | [libretro/mupen64plus-libretro-nx](https://github.com/libretro/mupen64plus-libretro-nx) | GPLv2 |
| Gambatte (GB/GBC) | [libretro/gambatte-libretro](https://github.com/libretro/gambatte-libretro) | GPLv2 |
| mGBA (GB/GBC/GBA) | [libretro/mgba](https://github.com/libretro/mgba) | MPL 2.0 |
| gpSP (GBA) | [libretro/gpsp](https://github.com/libretro/gpsp) | GPLv2 |
| PCSX ReARMed (PS1) | [libretro/pcsx_rearmed](https://github.com/libretro/pcsx_rearmed) | GPLv2 |

Also: the [libretro](https://www.libretro.com/) API and libretro-common, box art from
[libretro-thumbnails](https://github.com/libretro-thumbnails/libretro-thumbnails) and
[GameTDB](https://www.gametdb.com/), and [devkitPro](https://devkitpro.org/) / libnx, SDL2 and Mesa.

## Source code

The BetterArch source code (frontend, runtime, and the BetterMelon patches) will be published in
this repository. Until then, it's available on request: open an issue and you'll get a copy.

## Legal

BetterArch does not include, download or link to any games, BIOS or firmware. Only use backups of
games and system files you own. BetterArch is not affiliated with or endorsed by Nintendo, Sony,
Microsoft, or the authors of the emulators listed above.
