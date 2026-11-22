# Download

*Everything you need to install Shattered Dimensions on Windows.*

## The latest version

Download the latest version from [the latest release](https://github.com/zeref843/shattered-dimensions-updates/releases/latest) of this repository (one zip file with its SHA-256 checksum) or from [shattereddimensions.com](https://shattereddimensions.com).

Shattered Dimensions is free. The download is one zip file published on our official GitHub release page, with its SHA-256 checksum beside it. Only download it from this page or from that release page: copies from anywhere else are not ours, are not signed, and will not receive updates.

## What you need

| Requirement | Details |
|---|---|
| Windows | Windows 10 or 11, 64-bit |
| Graphics | A graphics card with Vulkan 1.3 support (NVIDIA, AMD or Intel; an up-to-date driver) |
| Disk space | About 1 GB free: the release folder and the game the setup builds |
| The game | A decrypted dump of **your own cartridge** of The Legend of Zelda: A Link Between Worlds, **US release** (.3ds or .cci) |
| Internet | Not needed to play. Only to download, and optionally to check for updates |

**Tested so far:** Windows 11 with an NVIDIA GeForce RTX 5080 Laptop GPU. More machines will be listed here as they are tested; if yours works (or does not), please tell us through [Support](../SUPPORT.md).

### About the game

Shattered Dimensions contains no game data and never will. The setup builds the game on your own computer from your own cartridge dump, and checks that it is the exact supported US release. You must obtain that dump lawfully, from a cartridge you own. We cannot provide game files or keys, and we do not link to them or to tools for obtaining them.

## Install it

1. **Unzip** the download into a folder you can write to, for example `Documents\Shattered Dimensions`. Keep the folder together: the `kit` folder inside it holds everything the setup needs.
2. **Run** `ShatteredDimensionsSetup.exe`. Nothing else has to be installed, and nothing is downloaded.
3. **Choose your dump.** The setup reads it (it never changes it) and checks that it is a 3DS cartridge image of the game, the US release, decrypted, and the exact supported version. If something is wrong, it says what in plain words.
4. **Build.** The setup translates and compiles the game on your computer: about a minute on a modern 8-core processor. You can follow the progress.
5. **Choose your preferences:** how you select items (hold a button, a radial wheel, or the classic window), widescreen 16:9 or the original 5:3, and our start menu. Everything can be changed later in the game.
6. **Play.** The setup adds a desktop shortcut and a Start menu entry.

The first launch may take a few seconds longer while your graphics driver prepares its shaders; later launches are faster.

## Where your files go

| What | Where |
|---|---|
| Your saves | `%APPDATA%\Shattered Dimensions\saves` |
| Your settings | `%APPDATA%\Shattered Dimensions\settings.ini` |
| The game the setup built | the release folder's `game` folder |

Uninstalling (Settings, Apps, or the setup) removes the game, its shortcuts and its entry, and **keeps your saves and settings**.

## Updates

When a new version is out, the game offers it on its start screen (you can turn this off). Updates are signed: the setup checks every update package and refuses any that is not ours or has been changed. Your saves are kept and backed up during every update.

## Check your download

Each release lists the SHA-256 checksum of its zip file. To check yours, open PowerShell in the folder with the download and run:

```
Get-FileHash .\ShatteredDimensions-*-Windows.zip -Algorithm SHA256
```

The value must match the one on the release page exactly. If it does not, delete the file and download it again from this page.

## Something not working?

- [The handbook](handbook/README.md): installation, graphics, controls and texture packs, step by step.
- [Support](../SUPPORT.md): fixes for common problems, and how to report a bug.
- [Updates](../UPDATES.md): every version, what changed, and the known issues.


---

> **Unofficial project.** Shattered Dimensions is an unofficial fan project. It is not affiliated with, endorsed or supported by Nintendo. It contains no game data: you need your own lawfully obtained copy of The Legend of Zelda: A Link Between Worlds (USA). Nintendo, The Legend of Zelda and A Link Between Worlds are trademarks of their owners.
