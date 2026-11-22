# Troubleshooting and FAQ

If your problem is not here, see [Support](../../SUPPORT.md): it walks you through the fix, or helps you report a bug.

## Setup

| Problem | Fix |
|---|---|
| "The dump is not decrypted" | Only decrypted dumps are accepted; the setup cannot decrypt files. |
| "Not the supported version" or "not A Link Between Worlds (US)" | Only the exact US release is supported. Other regions, revisions and modified files are refused. |
| "The kit is incomplete" | Unzip the whole download again and keep the `kit` folder next to the setup. |
| The build fails | The setup shows which step failed and why. Make sure the folder is writable (not in `Program Files`) and that you have about 1 GB free, then choose **Rebuild**. |
| The setup asks me to go through everything again | Only after the dump changed (a different file, or the same file modified). Otherwise it opens on its home page. |

## Graphics and performance

| Problem | Fix |
|---|---|
| The game does not start, or finds no suitable graphics card | Update your graphics driver. A card with Vulkan 1.3 is required. |
| Stutters when entering an area | Normal the first time each area is seen (shaders and enhanced textures are prepared, then kept). If it persists: turn off ray-traced shadows, then lower the resolution inside. |
| Below 60 frames a second | Choose a lower preset (F10, Advanced graphics). Extreme needs a very strong card. |
| An option is greyed out | Your PC cannot use it; the window says why (for example ray tracing needs hardware ray tracing). |
| Frame generation does nothing | It needs a supported NVIDIA card, applies from the next start, and works only while the window has focus. |
| Texture packs do not show | HD and 4K textures switch packs off: choose **The game's own** textures. Check the pack's status in F10, Texture packs. |
| The picture has bars at the sides | That is the original 5:3 shape; choose widescreen 16:9 (at 2x resolution and above). |

## Sound

| Problem | Fix |
|---|---|
| No sound | Check Windows' volume mixer and the default output device; the game uses the default device. |
| A brief crackle when pausing | A known small glitch on some systems, being worked on. |

Some of the original's room echo is our own recreation of the 3DS's sound effects, tuned by ear, so it may differ slightly from a real 3DS.

## Controllers and controls

| Problem | Fix |
|---|---|
| My controller does nothing | It must be one that Windows and SDL recognise as a gamepad (Xbox, PlayStation, Switch, 8BitDo and many more). An unknown joystick with no mapping is not used yet: please tell us which one through Support. |
| The wrong controller is active | The controller you used last is the active one: press a button on the one you want. |
| A key or button does the wrong thing | F10, controls: remap it, or reset the layout to its defaults. |
| The stick drifts or feels slow | F10, controls: raise the inner dead zone, or change the sensitivity and curve. |

## Saves

| Question | Answer |
|---|---|
| Where are my saves? | `%APPDATA%\Shattered Dimensions\saves` |
| Can an update delete them? | No. Updates keep your saves and back them up first. |
| Can a crash corrupt them? | No: saves are written completely or not at all. At most the last second before a crash is lost. |
| How do I back them up? | Copy the `saves` folder somewhere safe while the game is closed. |
| Can I use my 3DS saves? | Not in this version. |

## Frequently asked questions

**Is Shattered Dimensions an emulator?**
No. The setup translates the game into a native Windows program on your PC and builds it, and our own engine runs it.

**Why do I need my own cartridge dump?**
Shattered Dimensions contains none of the game. It only works with your own lawfully obtained copy, and we cannot provide one.

**Does it need the internet?**
No, except to download it and, if you leave it on, to check for updates (the start screen offers a new version when there is one).

**Is it free?**
Yes. Download it only from this website or its official GitHub release page: other copies are not ours, are not signed and do not get updates.

**Will it come to other platforms?**
We are working on it. Each platform will be announced on this website first.

**Can I change the controls, the HUD or the picture?**
Yes, all in the settings window: press F10.


---

> **Unofficial project.** Shattered Dimensions is an unofficial fan project. It is not affiliated with, endorsed or supported by Nintendo. It contains no game data: you need your own lawfully obtained copy of The Legend of Zelda: A Link Between Worlds (USA). Nintendo, The Legend of Zelda and A Link Between Worlds are trademarks of their owners.
