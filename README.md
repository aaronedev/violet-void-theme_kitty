# Violet Void Theme - kitty

Violet Void theme for kitty — a dark, vibrant terminal theme with purple and cyan accents.

## Preview

An interactive color preview is available at [`preview.html`](preview.html) — open it in any browser to see the full palette and a simulated terminal using the theme colors.

## Installation

### Option 1: Copy the config file

```bash
# Create kitty config directory if it doesn't exist
mkdir -p ~/.config/kitty

# Copy the theme file
cp violet_void.conf ~/.config/kitty/

# Add this line to your ~/.config/kitty/kitty.conf:
include violet_void.conf
```

### Option 2: Symlink (for development)

```bash
ln -s /path/to/violet_void.conf ~/.config/kitty/violet_void.conf
```

### Option 3: Via the monorepo

The theme is part of the [Violet Void](https://github.com/aaronedev/violet-void-monorepo) theme ecosystem. Clone the monorepo and symlink or copy the theme file.

## Colors

| Name | Hex | Usage |
|------|-----|-------|
| background | `#0f0f0f` | Main background |
| foreground | `#e7e7e7` | Main text |
| cursor | `#e7e7e7` | Cursor color |
| cursor_text | `#0f0f0f` | Text under cursor |
| selection_bg | `#191919` | Selected text background |
| selection_fg | `#e7e7e7` | Selected text foreground |
| url_color | `#00fff9` | Clickable URLs |

### Tabs

| Element | Background | Foreground |
|---------|------------|-------------|
| active_tab | `#29adff` | `#181818` |
| inactive_tab | `#222222` | `#383838` |

### Borders

| Element | Color |
|---------|-------|
| active_border | `#29adff` |
| inactive_border | `#222222` |

### Standard Colors (0-7)

| Index | Color | Hex |
|-------|-------|-----|
| 0 (black) | | `#181818` |
| 1 (red) | | `#ff004b` |
| 2 (green) | | `#42ff97` |
| 3 (yellow/magenta) | | `#7c60d1` |
| 4 (blue) | | `#29adff` |
| 5 (magenta) | | `#fd007f` |
| 6 (cyan) | | `#00fff9` |
| 7 (white) | | `#e7e7e7` |

### Bright Colors (8-15)

| Index | Color | Hex |
|-------|-------|-----|
| 8 | | `#333333` |
| 9 | | `#ff1a67` |
| 10 | | `#42ffad` |
| 11 | | `#d0a9e5` |
| 12 | | `#70c8ff` |
| 13 | | `#fd0098` |
| 14 | | `#b6e3ff` |
| 15 | | `#e7e7e7` |

### Extended Colors (16-17)

| Index | Hex |
|-------|-----|
| 16 | `#fa9f80` |
| 17 | `#ff004b` |

## Configuration Tips

### Customize tab colors

Add to your `kitty.conf` after the include:

```ini
# Override tab colors
active_tab_background #7c60d1
active_tab_foreground #e7e7e7
```

### Adjust cursor thickness

```ini
# Thicker cursor
cursor_shape block
cursor_thickness 3
```

## License

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

This theme is released under the [MIT License](LICENSE).

## Links

- [Violet Void Monorepo](https://github.com/aaronedev/violet-void-monorepo)
- [Upstream (Neovim plugin)](https://github.com/folke/violet-void.nvim)

---

Part of the **Violet Void** theme ecosystem — a consistent dark theme across terminals, editors, and applications.
