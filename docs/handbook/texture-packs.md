# Texture packs

A texture pack replaces pictures in the game with new ones. You need nothing but Shattered Dimensions, an image editor that saves PNG, and optionally a zip program (Windows has one built in).

## How packs work

- A pack is a **folder** or a **.zip** of one, in `%APPDATA%\Shattered Dimensions\texture-packs`.
- Inside are PNG pictures, each **named after the texture it replaces**. The name comes from the texture's own data, so it never changes between versions of Shattered Dimensions.
- Pictures are read the first time the game draws them, in the background, so even large packs do not slow loading.
- A pack can change two things: **the game's own textures** (the world, characters, items, the map, the hearts), and, for packs made for Shattered Dimensions, **our own interface** (the rupee counter and the energy gauge, so far).

**Packs are not used while HD or 4K textures are on** (see [Graphics](graphics.md#textures)). Choose **The game's own** textures to use packs.

## Installing and managing packs

1. Put the pack's folder or `.zip` into `%APPDATA%\Shattered Dimensions\texture-packs`. A zip works as it is: there is no need to unzip it.
2. In the game, press **F10** and open **Texture packs**. Every pack found is listed with its name, type, status and number of pictures.

| In the Texture packs section | What it does |
|---|---|
| The checkbox beside a pack | Switches that pack on or off |
| The arrows | Change the order: a pack higher in the list wins when two replace the same texture |
| Reload | Reads the packs again, so a changed picture shows at once |
| Hold to see the original textures | Shows the game's own pictures while held, to compare |
| Dump textures | Saves each texture the game draws, for making your own pack (below) |
| Open the packs folder | Opens the folder in Explorer |

To remove a pack, switch it off, or delete its folder or zip from the packs folder.

## Packs made for 3DS emulators

Packs made for A Link Between Worlds in 3DS emulators (Citra, Azahar) work as they are: drop the folder or zip in. Supported are packs whose `pack.json` uses the emulators' current naming (the default when the file exists): files named `tex1_<width>x<height>_<hash>_<format>.png`, or listed in the `pack.json`. Older packs without a `pack.json` used a different naming that is not supported yet; the pack report lists them. DDS and KTX pictures are planned for a later version.

**3DS packs can only change the game's textures, never our interface.**

## Making your own pack

### 1. Dump the textures

In the settings window (**F10**, **Texture packs**), turn on **Dump textures** and play. Every texture the game draws is saved once as a PNG in `%APPDATA%\Shattered Dimensions\texture-dump`. Go wherever the textures you want appear; turn the dump off when you are done. The dumped pictures come from your own copy of the game: keep them on your computer and do not share them.

### 2. Find the texture

Each file is named after the texture:

```
sd_<width>x<height>_<hash>_<format>.png
sd_16x16_13A407DCF5FE31C1_RGBA4.png
```

Browse the folder with large thumbnails. **Keep the file name exactly as it is.**

### 3. Paint the replacement

- **Size:** the original's size, or 2 to 8 times it (for example 64x64 for a 16x16 texture) for the sharpest result. Another size of the same shape also works; it is scaled to the nearest whole multiple.
- **Transparency** is kept.
- **Orientation:** paint it the way it appears in the dump.

Only use art you made yourself or have the right to use.

### 4. Make the pack

Make a folder in `texture-packs` and put your PNGs anywhere inside it, in sub-folders if you like. Files with other names are ignored, so notes can stay in the folder. Press **Reload** to see your changes at once.

### 5. Restyle our interface (optional)

Our own interface is not a game texture, so it has no dump name. A pack names the pieces it replaces in a `pack.json` file at its top:

```
{
  "pack_format": 1,
  "name": "My Blue HUD",
  "id": "yourname.my-blue-hud",
  "version": "1.0",
  "author": "Your name",
  "description": "A blue rupee and a teal energy gauge.",
  "replaces": {
    "sd:hud/rupee/gem": "rupee_gem.png",
    "sd:hud/energy/fill": "energy_fill.png"
  }
}
```

| Name | What it is | Suggested size |
|---|---|---|
| `sd:hud/rupee/gem` | the rupee beside the counter | 64 x 96 |
| `sd:hud/rupee/frame` | the counter's background | 256 x 64 |
| `sd:hud/energy/empty` | the energy gauge's background | 512 x 40 |
| `sd:hud/energy/fill` | the gauge's fill; its left part shows as much as there is energy | 512 x 40 |
| `sd:hud/energy/frame` | the gauge's frame, transparent inside | 512 x 40 |

`"pack_format": 1` is required for `"replaces"`. Name, version, author and description are shown in the manager.

### 6. Share it

Zip the pack's folder (right-click, Compress to ZIP). Players drop the zip into their packs folder without unpacking it. Share only pictures you made: never the dumped originals.

## When something is wrong

The game always keeps running: a picture that cannot be used is drawn as the original.

- A **pop-up** appears when a pack cannot be used, or only partly. It shows once.
- The **Texture packs** section shows each pack's status; **Details** lists every file not used and why.
- `texture-packs\report.txt` holds the same.

| The report says | What to do |
|---|---|
| is not a PNG picture | Save it again as PNG (not renamed from JPG or WebP) |
| larger than 8192 on a side | Use a smaller multiple of the original size |
| could not be unpacked, cut short | The zip is damaged: make it again |
| named for another texture size or format | Copy the name from the dump again |
| not the shape of the texture it replaces | Keep the original proportions |
| resized to a whole multiple | It works; for the sharpest result, use exactly 2, 3, 4 times the size |
| is not a name Shattered Dimensions knows | Check the name against the table above |
| "replaces" but no "pack_format": 1 | Add `"pack_format": 1` to `pack.json` |

Packs are checked for safety: at most 100,000 files, each at most 256 MB and 8192 pixels on a side; zip entries with unsafe names, possible decompression bombs, encryption or unusual compression are refused. Nothing in a pack is ever unpacked to your disk.


---

> **Unofficial project.** Shattered Dimensions is an unofficial fan project. It is not affiliated with, endorsed or supported by Nintendo. It contains no game data: you need your own lawfully obtained copy of The Legend of Zelda: A Link Between Worlds (USA). Nintendo, The Legend of Zelda and A Link Between Worlds are trademarks of their owners.
