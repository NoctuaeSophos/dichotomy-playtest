# Credits

**Dichotomy** by NoctuaeSophos.

Built with [Godot Engine](https://godotengine.org) 4.7 (MIT License, © the Godot Engine contributors).

## Pixel look

The pixel look (`scripts/pixel_look.gd`, `shaders/pixel_post.gdshader`, `shaders/toon.gdshader`) is a port of the
rendering of **eco** by teq ([Teqed](https://github.com/Teqed), [github.com/Teqed/eco](https://github.com/Teqed/eco)),
offered for use by its author: its pixel pipeline (a whole-number pixel scale, a one-texel padded render and a camera
snapped to whole texels, with the remainder shown as a sub-pixel shift), its post pass (plane-predicted depth outlines,
convex-corner highlights with crease suppression, outline tint, highlight gain and lift, colour quantising, and its
debug views), and its toon shading (shadow/mid/highlight ramps by the sun's lambert term with jitter, eco's night
colours, and lamp light stepped into three bands). Where the port departs from eco (Dichotomy's own camera angle,
ramps derived from each surface's colour, Godot's lights in place of eco's light grid) is noted in those files.
eco is released under the MIT License:

```
MIT License

Copyright (c) 2026 teq

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Controller and keyboard icons

Button prompts use the **Controller Icons** add-on by rsubtil
([github.com/rsubtil/controller_icons](https://github.com/rsubtil/controller_icons), commit 24281f8, MIT License; its full
license is in `addons/controller_icons/LICENSE`), which detects the controller type and supplies the icons. The icon art is
**Xelu's FREE Controllers & Keyboard PROMPTS** by Nicolae (XELU) Berbece ([thoseawesomeguys.com/prompts](https://thoseawesomeguys.com/prompts/)),
released under CC0, with extra icons contributed to the add-on under CC0.

## Characters

The thief and the guards are CC0 models by **Quaternius** ([quaternius.com](https://quaternius.com)): the Rogue from
*LowPoly RPG Characters* (Nov 2020) and the Blue Soldier from the *Ultimate Animated Character Pack* (Nov 2019), both
released under CC0 1.0 (licence notes in `assets/characters/quaternius/`). Dichotomy recolours them, makes them taller
and broader with smaller heads and arms so they read at its scale, and poses them in code. The original box-built
figures remain, behind "Classic figures" in the debug menu.

Ghost looks on deck (the debug menu's "Ghost look"; the sheet is the default): Kenney's ghost from the *Graveyard Kit*
(CC0), Quaternius' *Ghost* and *Ghost Skull* (CC0, via Poly Pizza), and the base body, witch and zombie from Quaternius'
*Ultimate Animated Character Pack* (CC0), in `assets/characters/ghosts/` with their licence notes.

## AI and tests

Guard and ghost AI can use **LimboAI** by Serhii Snitsaruk and contributors
([github.com/limbonaut/limboai](https://github.com/limbonaut/limboai), v1.8.1, MIT License; full license in
`addons/limboai/LICENSE.md`; its logo is CC BY 4.0, see `addons/limboai/LOGO_LICENSE.md`). Tests run on **gdUnit4** by
Mike Schulze and contributors ([github.com/godot-gdunit-labs/gdUnit4](https://github.com/godot-gdunit-labs/gdUnit4),
v6.2.3, MIT License), which isn't part of the game builds.

## Inspirations

Boktai (pace, isometric stealth, pressing against walls and tapping), Persona 3 Portable (two worlds), and
Mark of the Ninja (stealth versus fear).
