# Getting started

## What Shattered Dimensions is

Shattered Dimensions is a native Windows engine for The Legend of Zelda: A Link Between Worlds. It is not an emulator: the setup translates the game from your own cartridge dump into a real Windows program and builds it on your PC, then runs it on our own engine and graphics renderer.

What that gives you:

- the game at high resolutions, up to 6 times the original inside the game, in a window or full screen;
- a widescreen 16:9 picture that shows more of the world, or the original 5:3 shape;
- one screen instead of two: the second screen becomes a live minimap, and its menus open as panels;
- keyboard, mouse and controller controls you can remap;
- optional HD and 4K texture enhancement, texture packs, and ray-traced shadows on capable graphics cards.

## What you need

- **Windows 10 or 11**, 64-bit.
- **A graphics card with Vulkan 1.3** (NVIDIA, AMD or Intel) and an up-to-date driver.
- **About 1 GB of free disk space.**
- **A decrypted dump of your own cartridge** of the game, **US release**, as a `.3ds` or `.cci` file. You must obtain it lawfully from a cartridge you own. Shattered Dimensions does not include, provide or link to game files, keys, or tools for obtaining them.

So far the game has been tested on one PC (Windows 11, NVIDIA GeForce RTX 5080 Laptop GPU). If you play on something else, we would like to hear how it runs: see [Support](../../SUPPORT.md).

## Installing

1. Download the zip from the [Download page](../download.md) and unzip it into a folder you can write to, such as `Documents\Shattered Dimensions`. Keep everything in that folder together.
2. Run `ShatteredDimensionsSetup.exe`. Nothing else is installed and nothing is downloaded.
3. **Choose your dump.** The setup reads it without changing it and checks four things: that it is a 3DS cartridge image, that it is A Link Between Worlds (US), that it is decrypted, and that it is the exact supported version. If a check fails, the setup says which one.
4. **Build.** The setup translates and compiles the game on your PC. On a modern 8-core processor this takes about a minute; you can watch its progress.
5. **Your preferences:**
   - **How you choose items:** hold a button, a radial wheel, or the classic window (see [Interface and controls](controls.md#choosing-items)).
   - **Picture shape:** widescreen 16:9 or the original 5:3.
   - **Our start menu:** a file screen in the style of the game, or the game's own.
   All of these can be changed in the game later.
6. **Play.** A desktop shortcut and a Start menu entry are made for you.

Running the setup again opens a home page with Play, Update (when a newer version has been installed), Preferences and Rebuild. It does not ask you to go through every step again.

## Your first launch

- The first start may take a few extra seconds while your graphics driver prepares its shaders. Later starts are faster.
- The game opens in a window that fits your screen, at 60 frames a second, at the resolution your screen suits (the **Normal** preset).
- Press **F10** for the settings window. Press **Alt+Enter** to switch between a window and full screen.

## Where your files go

| What | Where |
|---|---|
| Saves | `%APPDATA%\Shattered Dimensions\saves` |
| Settings | `%APPDATA%\Shattered Dimensions\settings.ini` |
| Control layouts | `%APPDATA%\Shattered Dimensions\input.ini` |
| Texture packs | `%APPDATA%\Shattered Dimensions\texture-packs` |
| The game the setup built | the release folder's `game` folder |

To open `%APPDATA%`, press Windows+R, type `%APPDATA%` and press Enter.

**Saves are protected.** Each save is written completely or not at all, so a crash or a power cut cannot leave a half-written save. At most the last second of writes before a crash can be lost; the previous save stays intact. Updates keep your saves and back them up first.

## Common startup problems

| What you see | What to do |
|---|---|
| The setup says the dump is not decrypted | The setup only accepts decrypted dumps of the US release. It cannot decrypt files itself. |
| The setup says the dump is not the supported version | Only one exact version is supported (it checks the file's SHA-256). Other regions and revisions are not supported. |
| The setup says its kit is incomplete | Unzip the whole download again, keeping the `kit` folder next to the setup. |
| The game does not start, or says no graphics card is suitable | Update your graphics driver. A card with Vulkan 1.3 is required. |

More in [Troubleshooting and FAQ](troubleshooting.md).


---

> **Unofficial project.** Shattered Dimensions is an unofficial fan project. It is not affiliated with, endorsed or supported by Nintendo. It contains no game data: you need your own lawfully obtained copy of The Legend of Zelda: A Link Between Worlds (USA). Nintendo, The Legend of Zelda and A Link Between Worlds are trademarks of their owners.
