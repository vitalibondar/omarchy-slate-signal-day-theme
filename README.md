# Slate Signal Day

A light Omarchy theme for people who read a lot of text on a small screen. Grey chassis, one blue that means something, and a text selection you can actually see. This is the day half of a pair. The night half is [Slate Signal Night](https://github.com/vitalibondar/omarchy-slate-signal-night-theme).

## Why it looks like this

I work on a 14" 1920x1080 ThinkPad and my eyesight is minus six. On that screen most light themes either glare or wash out. So the ground here is off-white (`#f3f4f6`) rather than pure white, body text sits at 15:1, and nearly everything else is grey. The only colour that carries meaning is the blue (`#16589f`): links, the accent, the border of the focused window. And because nothing else competes with it, you spot it without looking for it.

Selection is a plain, fairly strong fill (`#97abc4`). I wanted a thin accent edge around the selected region. But no terminal or editor that Omarchy themes exposes one, so the fill got deeper instead. Selected text stays above 7:1. The fill itself sits at about 2:1 against the page, which is on purpose: a single colour cannot be a 3:1 region and hold 7:1 text at the same time, and I chose readable text.

## Install

```sh
omarchy theme install https://github.com/vitalibondar/omarchy-slate-signal-day-theme.git
```

Two wallpapers ship with the theme. And they are part of it, not an afterthought: `01` is a damask tile for everyday use, so any gap between tiled windows lands on full detail. `02` is a bouquet with more empty space, better for the lock screen or as a change. `omarchy theme bg next` cycles between them.

## The pair

Day and Night use the same hues with the lightness order reversed. If you switch them by sunrise and sunset, keep the geometry (font size, window border, corner rounding) in a machine-level file rather than in the theme, so nothing jumps when the theme changes. Those files, the contrast checker and the design notes live in [slate-signal](https://github.com/vitalibondar/slate-signal).

## Numbers

Measured on the hex values with the checker from the slate-signal repo, WCAG 2.x.

| Pair | Ratio |
|---|---|
| body text / background | 15.4 |
| emphasis / background | 17.8 |
| muted text / background | 5.8 |
| accent / background | 6.5 |
| selected text / selection | 8.3 |
| selection / background | 2.1 (intentional, see above) |

## Status

New. It went onto my own machine on 3 September 2026, and previews will follow once I have lived with it for a bit. If something reads badly on your screen, open an issue and say which screen.

## Credits

Palette and decisions were worked out in Claude Design against Omarchy 4.0.2 templates, and installed with Claude Code. The wallpapers were generated with ChatGPT for this theme. MIT, wallpapers included.
