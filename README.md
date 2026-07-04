# ⚡ Neon Terminal 2030

A futuristic **2030 terminal-style** color theme for VS Code, inspired by modern AI CLIs (like Claude CLI).
Deep-space dark background, neon accents, and **every syntax element gets its own distinct color** — so reading code feels like reading a live terminal stream.

![Neon Terminal 2030 preview]

## ✨ Variants
- **Neon Terminal 2030** — deep blue-black canvas (`#0A0D14`)
- **Neon Terminal 2030 (Deep Void)** — pure black OLED canvas (`#000000`)
- **Neon Terminal 2030 (Daylight)** — soft light canvas (`#FBFCFE`) with darkened neon accents 🌞

## 🎨 Color Language

Each role has one signature color — nothing is reused arbitrarily:

| Element | Color | Hex |
|---|---|---|
| Keywords / control flow | 🩷 neon magenta | `#FF4D9D` |
| Storage / modifiers | 🌸 pink (italic) | `#FF7AB8` |
| Strings | 🟩 mint | `#34F5C5` |
| Numbers / constants | 🟧 amber | `#FFB84D` |
| Booleans / `this` / null | 🟠 coral | `#FF7A5C` |
| Functions | 🔵 sky blue | `#5BC0FF` |
| Classes / types | 🟣 violet | `#C792FF` |
| Object properties | 💧 light cyan | `#9BD8FF` |
| Parameters | 🍑 peach (italic) | `#FFAFA0` |
| Operators | 🩵 bright cyan | `#6EE7FF` |
| Attributes / decorators | 🟡 gold (italic) | `#FFD93D` |
| Comments | 🌫️ muted slate (italic) | `#445069` |
| Variables / text | ⚪ soft white | `#C6D2E2` |

Fully styled surfaces include **sticky scroll**, **inlay hints**, **ghost text / inline AI suggestions**, **bracket-pair guides**, **merge conflicts**, **notebooks**, the **command center**, **charts**, **minimap markers**, **testing/debug icons**, and rainbow bracket-pair colors. The integrated terminal ships a full neon ANSI palette.

## 🚀 Install / Try Locally

1. Copy this folder into your VS Code extensions dir, or open it and press **F5** to launch an Extension Development Host.
2. `Ctrl/Cmd + K` then `Ctrl/Cmd + T` → pick a **Neon Terminal 2030** variant.

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
