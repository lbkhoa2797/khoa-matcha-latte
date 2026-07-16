# Khoa's Matcha theme

## This repo include the color scheme for VScode and iTerm2

# Khoa Matcha Theme (Adapted from Matcha-zen theme) 🍵

A matcha-latte inspired color scheme — Since it's my favorite.

Available for both **iTerm2** and **VS Code**. Found some variants but not quite as I like so I just make one myself.

## Preview

| Background | Foreground | Accent |
|---|---|---|
| `#F5F7EA` | `#354029` | `#4E8C2E` |

### iterm2
<img width="600" height="400" alt="iTerm2-ss" src="https://github.com/user-attachments/assets/0287b413-a49b-46f4-b585-9f992bbe344a" />


### VScode
<img width="500" height="400" alt="VS-code-ss" src="https://github.com/user-attachments/assets/8e45713b-5250-47aa-bdad-adfc07bd3807" />

## Contents

```
.
├── iterm2-files/
│   └── matcha-latte.itermcolors      # iTerm2 color preset
└── vscode-files/
    ├── themes/
    │   └── matcha-latte-color-theme.json
    ├── package.json
    ├── khoa-matcha-theme-0.0.1.vsix  # pre-packaged, ready to install
    ├── CHANGELOG.md
    └── vsc-extension-quickstart.md
```

## Installing the iTerm2 theme

1. Download [`matcha-latte.itermcolors`](iterm2-files/matcha-latte.itermcolors)
2. Open **iTerm2** → **Settings** → **Profiles** → **Colors** tab
3. Click **Color Presets…** (bottom right) → **Import…**
4. Select `matcha-zen.itermcolors`
5. Open **Color Presets…** again and select **matcha-zen** to apply it

## Installing the VS Code theme

### Option A — Install the packaged `.vsix` directly (fastest)

1. Download [`khoa-matcha-theme-0.0.1.vsix`](vscode-files/khoa-matcha-theme-0.0.1.vsix)
2. Install it:
   ```bash
   code --install-extension khoa-matcha-theme-0.0.1.vsix
   ```
3. In VS Code: `Cmd/Ctrl+K Cmd/Ctrl+T` → select **Matcha Latte**

### Option B — Clone and package yourself

```bash
git clone https://github.com/lbkhoa2797/khoa-matcha-latte.git
cd khoa-matcha-latte/vscode-files
npm install -g @vscode/vsce
vsce package
code --install-extension khoa-matcha-theme-0.0.1.vsix
```

### Option C — Symlink for live editing (no repackaging needed)

```bash
git clone https://github.com/lbkhoa2797/khoa-matcha-latte.git ~/.vscode/extensions/khoa-matcha-theme
```
Restart VS Code and the theme is picked up automatically. Future `git pull`s update it in place.

### Set as default theme

Add to your VS Code `settings.json`:
```json
"workbench.colorTheme": "Matcha Latte"
```

## Development

To tweak the VS Code theme:
1. Open `vscode-files/` in VS Code
2. Edit `themes/matcha-latte-color-theme.json`
3. Press `F5` to launch an Extension Development Host and preview changes live
4. Re-run `vsce package` when you're happy, to produce an updated `.vsix`

## License

MIT — free to use, modify, and share.
