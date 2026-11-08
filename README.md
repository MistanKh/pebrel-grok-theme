# Grok Theme for Pebrel

Two Pebrel themes built around a restrained graphite/ivory palette: near-black
chrome, warm text, and one desaturated steel accent. Both are colors-only and
use the native Pebrel theme format.

- **Grok Obsidian** — dark. Chrome sits at `#0C0C0C`, terminal at `#101010`.
- **Grok Parchment** — light. Warm paper chrome with the same muted syntax palette.

![Grok Obsidian](previews/grok-obsidian.png)

![Grok Parchment](previews/grok-parchment.png)

## Install

Once listed in the Pebrel Community catalog:

1. Open **Settings → Appearance → Community themes**.
2. Install **Grok Obsidian** or **Grok Parchment**.
3. Select it from the theme picker.

Manual install from a release ZIP:

```sh
pebrel theme import grok-obsidian.pebrel-theme.zip
```

Then choose the theme in **Settings → Appearance**.

## Palette

| Role | Obsidian | Parchment |
| --- | --- | --- |
| Chrome / sidebar | `#0C0C0C` | `#F4F3F0` |
| Tab cards | `#131313` | `#EFEEEB` |
| Terminal | `#101010` | `#FBFBF9` |
| Text / muted | `#E6E4DF` / `#9A9892` | `#242422` / `#686866` |
| Accent, cursor | `#A9BCCB` | `#4C6478` |
| Keyword | `#A6B8C6` | `#4C6478` |
| Function | `#D4C8B4` | `#4E6A5A` |
| String | `#AEBE9C` | `#5C6B3F` |
| Type | `#9DBFB6` | `#2F5F5A` |
| Number | `#C7A9A0` | `#8A5A52` |

The dark theme keeps the left tabs pane one step darker than the terminal, like
the reference Grok shell. `ui.background` controls the chrome; `ui.sidebar`
controls tab-card surfaces.

Tested with Pebrel 2.4.0 on Windows 11 (x64). Colors-only; no shaders,
wallpapers, or external resources.

## Build

Requires Pebrel's `theme` command:

```sh
pebrel theme pack --output dist/grok-obsidian.pebrel-theme.zip \
  --author MistanKh --license MIT themes/grok-obsidian.pebrel-theme.json

pebrel theme check dist/grok-obsidian.pebrel-theme.zip
```

Release assets follow the Community catalog contract: a versioned tag with
`.pebrel-theme.zip` files.

## License

MIT. Unofficial theme, not affiliated with xAI.
