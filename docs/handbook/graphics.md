# Graphics and performance

All graphics settings are in the settings window: press **F10** in the game and open **Advanced graphics**. Most changes apply at once; ray-traced shadows and frame generation apply from the next start, and the window says so.

Options your PC cannot use are shown greyed out, with the reason.

## Presets

A preset sets the resolution, the frame rate, ray-traced shadows and frame generation in one choice. Change any setting afterwards and the preset shows **Custom**.

| Preset | What it sets |
|---|---|
| **Potato** | 2x resolution (480 lines), 60 frames a second, no advanced effects. Runs on almost anything. |
| **Normal** | The resolution that fits your screen, 60 frames a second. This is how the game starts. |
| **High** | At least 4x resolution (960 lines), and as many frames as your screen can show. |
| **Ultra** | 5x resolution (1200 lines), ray-traced shadows, frame generation, uncapped frame rate. |
| **Extreme** | 6x resolution (1440 lines), ray-traced shadows with the softest edges, frame generation, uncapped. Needs a stronger card than an RTX 5080 laptop. |

Whatever you choose, **the game itself always runs at its own 60 steps a second**: a higher frame rate makes the picture smoother; it never speeds up the game.

## Resolution inside

The **resolution inside** is how many lines the world is drawn with: **Auto** (fits your screen) or 1x to 6x the original 240 lines (1x is the 3DS's own; 4x is 960 lines; 6x is 1440). Higher is sharper and needs more from your graphics card.

## Display

- **Windowed:** a normal window you can resize.
- **Borderless:** fills the screen without changing your display's mode.
- **Fullscreen:** switches your display to the chosen resolution and refresh rate.

**Alt+Enter** switches between a window and full screen at any time.

## Frame rate

- **60 (the game's own):** the steadiest choice.
- **Match the screen:** as many frames as your display shows (for example 120 or 144).
- **Uncapped:** as fast as your PC can draw.

## Picture shape

- **Widescreen 16:9:** shows more of the world at the sides, never stretched. Available at 2x resolution and above.
- **Original 5:3:** the 3DS's own shape, with bars at the sides.

## Textures

Four kinds of texture are available, and **only one is active at a time**:

| Choice | What it does |
|---|---|
| **The game's own** | The original textures. Texture packs are used when you have any installed and enabled. |
| **HD textures (2x)** | Every texture enhanced to twice its size by our own upscaler: sharper edges, no halos. |
| **4K textures (4x)** | Every texture enhanced to four times its size. |
| **Texture packs** | Pictures made by people for the game: see [Texture packs](texture-packs.md). |

**HD and 4K textures switch texture packs off** while they are on. Each texture is enhanced the first time it appears and then kept on disk, so it is only ever done once; until then, for a moment, the original is shown.

**Sharp map and menus** (on by default) enhances the map and the Items and Gear screens so they stay crisp at high resolutions. It works with every choice above.

## Ray-traced shadows

On graphics cards with hardware ray tracing, the world can cast real shadows from the sun and from the lights of rooms, caves and dungeons. The setting asks you to confirm a short warning the first time.

- **Shadow edge quality:** 4, 8 or 16 rays. More rays give softer edges and cost more.
- **Sun for shadows:** from above (the default, which suits the game's tilted buildings) or the game's own light.

Ray-traced shadows are the most demanding option. If the game stutters when you change areas, turn them off first.

## Frame generation

On NVIDIA graphics cards that support DLSS Frame Generation, extra frames can be generated between the game's own, for a smoother picture. It works only while the window has focus. Choose how many frames are shown per game frame; a change applies from the next start.

## What to choose for your PC

- **A modest or older PC, or integrated graphics:** Potato or Normal, with the game's own textures.
- **A mid-range graphics card:** Normal or High; HD textures if you like.
- **A strong graphics card:** High or Ultra; 4K textures and ray-traced shadows if it keeps 60.
- **If you notice stutters:** turn off ray-traced shadows first, then step down the resolution inside.

The first time you enter an area, the game may take a moment longer while new shaders and enhanced textures are prepared; after that they are kept.


---

> **Unofficial project.** Shattered Dimensions is an unofficial fan project. It is not affiliated with, endorsed or supported by Nintendo. It contains no game data: you need your own lawfully obtained copy of The Legend of Zelda: A Link Between Worlds (USA). Nintendo, The Legend of Zelda and A Link Between Worlds are trademarks of their owners.
