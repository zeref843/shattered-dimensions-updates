# Updates

*Every version of Shattered Dimensions, what changed, what is known, and what comes next.*

## Versions

Every version, newest first, with what is new, what was fixed, what changed and what was removed. Times are in UTC, the moment each version was published.

### Version 1.1.2 (latest), 22 November 2026, 20:37 UTC

**How to get it:** on 1.1.1, your game offers it with the notice at the top of the file list. On 1.0.0 or 1.1.0, download it once from the [Download page](docs/download.md) and install it over your current version; those versions cannot show the offer. Your saves are kept: they live in your user folder, not in the game folder.

- **New:** nothing.
- **Fixed:** a new version could stay hidden for up to a day, because the game asked for updates at most once a day.
- **Changed:** the game now checks for updates **every time it starts**, in the background, so a new version is offered as soon as you open the game. Turning "Check for updates" off still stops it. The setup's checkbox now reads "Check for updates (when the game starts, from GitHub; nothing about you is sent)".
- **Removed:** the once-a-day limit on update checks.

### Version 1.1.1, 22 November 2026, 19:19 UTC

- **New:** an **update notice that is always on screen**: a gold-framed notice at the top right of the file list. It shows the new version, then the download progress, then "close the game and install it (your saves are kept)", or a failure with "try again". Press Select or click it to act. It is tested at ten window shapes, from 640x480 to ultrawide and full screen, and no version can be released unless that test passes.
- **Fixed:** in 1.0.0 and 1.1.0 the update offer was drawn below the bottom of the screen, so players never saw it.
- **Changed:** nothing else.
- **Removed:**
  - the old one-line update offer at the bottom of the file list;
  - versions 1.0.0 and 1.1.0 were withdrawn from download the same day (22 November 2026, about 19:24 UTC), because their update offer was drawn off the bottom of the screen. They were not bad copies: we missed it while working on everything else, and we want everyone to have the best experience possible. Their changes are part of every later version.

### Version 1.1.0 (withdrawn), 22 November 2026, 17:13 UTC

No longer available to download; 1.1.2 includes everything below.

**Why it was withdrawn:** this was never a bad copy, and nothing was wrong with the game in it. While we were working on everything else for the release, we missed that its update offer was drawn below the bottom of the screen, so players on it would never see that a new version was out. We took it down so no one could get stuck on a version that cannot tell them about updates: we want everyone to have the best experience possible.

- **New:** nothing.
- **Fixed:** the energy gauge under the hearts showed from the first walk out of Link's house. It now stays hidden until Ravio hands Link the Bow, as in the original game, and fades in as the game's own gauge does. Existing saves follow the game's own progress.
- **Changed:** **Licence 1.1**: the copyright holder is named as Zeref843 (WeaverLume Studios), and the ownership wording is clearer. The other terms are unchanged.
- **Removed:** nothing.

### Version 1.0.0 (withdrawn), 22 November 2026, 11:56 UTC

The first public release. No longer available to download; 1.1.2 includes everything below.

**Why it was withdrawn:** this was never a bad copy, and nothing was wrong with the game in it. While we were working on everything else for the release, we missed that its update offer was drawn below the bottom of the screen, so players on it would never see that a new version was out. We took it down so no one could get stuck on a version that cannot tell them about updates: we want everyone to have the best experience possible.

- **New:**
  - a native Windows engine that runs the game from your own cartridge dump, translated and built on your PC by the setup;
  - high resolutions, up to 6 times the original, in a window, borderless or full screen, at 60 frames a second or matched to your screen;
  - widescreen 16:9 that shows more of the world, or the original 5:3;
  - one screen: the live minimap in a corner, the map, Items and Gear as panels, and the hearts, rupees and energy gauge rearranged for one screen;
  - choosing items your way: hold a button, a radial wheel, or the classic window;
  - keyboard, mouse and controllers, fully remappable, with on-screen buttons that follow the device you use;
  - HD and 4K textures from our own upscaler, and a sharp map and menus at any resolution;
  - texture packs, including packs made for 3DS emulators and packs that restyle the new interface;
  - ray-traced shadows and DLSS Frame Generation on graphics cards that support them;
  - safe saves, written completely or not at all, kept and backed up through every update;
  - signed updates offered in the game.
- **Fixed, Changed, Removed:** nothing; this was the first version.

## Known issues

These are known in the current version. If you meet one, you do not need to report it; if you meet something else, please use [Support](SUPPORT.md).

| Area | What you may notice |
|---|---|
| Testing | Shattered Dimensions has been tested on one PC so far (Windows 11, NVIDIA RTX 5080 Laptop GPU). Results on other hardware are welcome. |
| Controllers | Tested with virtual controllers and the keyboard; real controllers are being tested. An unknown joystick with no built-in mapping is not used yet. |
| Performance | The first time each area is entered, one frame can take longer while new shaders and textures are prepared; it is kept afterwards. With ray-traced shadows on, entering an area costs a little more. |
| Presets | Extreme needs a graphics card stronger than an RTX 5080 laptop to hold full speed. |
| Sound | The 3DS's built-in room echo is our own recreation, tuned by ear. A brief crackle can occur when pausing on some systems. |
| Frame generation | Works only while the game window has focus. |
| Saves | 3DS saves cannot be imported. |

## What comes next

| Version | Plan |
|---|---|
| 1.1.x | Fixes for anything urgent found after the release, whenever needed. |
| **Android** | **In active development:** Shattered Dimensions as a native Android app, with the same engine, menus, settings and saves as on Windows, plus touch controls and controller support. It runs on our test phone and we are now making it fast and smooth. Not available yet and no release date; it will be announced here first. |
| **1.5** | **NEXUS Watch** (planned): an optional, off-by-default way to send us reports of crashes and errors (see below), and improvements from players' feedback. |
| Later | More platforms (each announced here first), and the community features on [Coming soon](COMING_SOON.md). New graphics technologies are being investigated; we will only list them here once they work. |

### NEXUS Watch (planned for 1.5)

NEXUS Watch will be an optional reporter built into the game. **It is not available yet, and nothing is collected today.** When it arrives:

- it will be **off unless you turn it on**, with a choice for each kind of report;
- it will report crashes, errors and problems the game detects, with the version, your graphics card and where in the game it happened;
- screenshots, if you allow them, will show the game's own picture only, never your desktop;
- nothing unnecessary will be kept on your computer, and nothing will be used for analytics or tracking;
- reports will travel encrypted to our reporting service. Like any internet connection, that service necessarily sees the connection's address while delivering a report; it will not keep it or use it to identify you.

The full privacy details will be published here before it is released.


---

> **Unofficial project.** Shattered Dimensions is an unofficial fan project. It is not affiliated with, endorsed or supported by Nintendo. It contains no game data: you need your own lawfully obtained copy of The Legend of Zelda: A Link Between Worlds (USA). Nintendo, The Legend of Zelda and A Link Between Worlds are trademarks of their owners.
