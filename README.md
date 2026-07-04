# ⚡ 2030

A futuristic **2030 terminal-style** color theme collection for VS Code, inspired by modern AI CLIs (like Claude CLI).
Deep-space backgrounds, neon accents, and **every syntax element gets its own distinct color** — so reading code feels like reading a live terminal stream.

![2030 preview]

## ✨ Variants

| Variant | Mood | Canvas |
|---|---|---|
| **2030** | signature neon on blue-black | `#0A0D14` |
| **2030 Void** | pure black OLED | `#000000` |
| **2030 Daylight** | soft light, darkened neons 🌞 | `#FBFCFE` |
| **2030 Solar** | warm ember — amber, gold, coral 🔥 | `#14100A` |
| **2030 Synthwave** | retro 80s — magenta, cyan, purple 🌆 | `#17132E` |
| **2030 Matrix** | green phosphor CRT 🟢 | `#030805` |
| **2030 Aurora** | cool arctic — teal, ice-blue, lavender ❄️ | `#0A1420` |

## 🎨 Color Language

Each syntax role has one signature color — nothing is reused arbitrarily. Roles map consistently across every variant (only the palette changes): keywords, storage/modifiers, strings, numbers, booleans, functions, classes/types, properties, parameters, operators, decorators, and comments each get a dedicated hue.

Fully styled surfaces include **sticky scroll**, **inlay hints**, **ghost text / inline AI suggestions**, **bracket-pair guides**, **merge conflicts**, **notebooks**, the **command center**, **charts**, **minimap markers**, **testing/debug icons**, and rainbow bracket-pair colors. The integrated terminal ships a full neon ANSI palette. Diagnostic and git colors (error red, warning amber, added green) stay meaningful in every variant — even the near-monochrome ones.

## 🛠 How the variants are built

All variants are generated from a single template so they stay structurally identical. Each is defined as a compact palette of roles in [build-themes.js](build-themes.js); running it expands every palette into a full theme file:

```bash
node build-themes.js
```

To add a new variant, add one palette object to the `PALETTES` array, run the script, and register it in [package.json](package.json) under `contributes.themes`.

## 🚀 Install / Try Locally

1. Copy this folder into your VS Code extensions dir, or open it and press **F5** to launch an Extension Development Host.
2. `Ctrl/Cmd + K` then `Ctrl/Cmd + T` → pick a **2030** variant.

### Package as a `.vsix`
```bash
npm install -g @vscode/vsce
vsce package
```
Then **Extensions → ⋯ → Install from VSIX…**

## 💡 Recommended settings
Set these for the best look:
```jsonc
{
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active",
  "editor.semanticHighlighting.enabled": true,
  "editor.fontLigatures": true,
  "editor.stickyScroll.enabled": true,
  "editor.cursorBlinking": "phase",
  "editor.cursorSmoothCaretAnimation": "on",
  "terminal.integrated.fontFamily": "JetBrains Mono, Fira Code"
}
```

---
Made for the year 2030, today. 🛸
