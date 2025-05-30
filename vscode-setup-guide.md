# 🧑‍💻 Brad's VS Code Setup Guide

This guide walks you through replicating my full Visual Studio Code setup, including my extensions, themes, icons, and editor settings. Everything here was hand-picked and manually set by me—no syncing or scripts.

---

## 1. 🎨 Theme and Icon Setup

### Color Theme

* **SynthWave '84 Min Darker Theme**

  * Search for: `fernaandojr.synthwave-remix-min-darker`
  * Apply via: `Settings > Theme > Color Theme`

### File Icon Theme

* **Catppuccin Frappé Icons**

  * Search for: `catppuccin.catppuccin-vsc-icons`
  * Apply via: `Settings > Theme > File Icon Theme`

### Product Icon Theme

* **Atom Material Product Icons**

  * Search for: `atommaterial.a-file-icon-vscode`
  * Apply via: `Settings > Theme > Product Icon Theme`

---

## 2. 🔌 Extensions to Install (Search & Install via Extensions Sidebar)

Search for and install the following extensions one by one:

```text
aaron-bond.better-comments
azemoh.one-monokai
catppuccin.catppuccin-vsc
be5invis.vscode-custom-css
chadalen.vscode-jetbrains-icon-theme
chakrounanas.turbo-console-log
dbaeumer.vscode-eslint
esbenp.prettier-vscode
eamodio.gitlens
formulahendry.code-runner
humao.rest-client
openai.chatgpt
github.copilot
gruntfuggly.todo-tree
oderwat.indent-rainbow
streetsidesoftware.code-spell-checker
usernamehw.errorlens
teabyii.ayu
wix.vscode-import-cost
```

---

## 3. ✨ Key Extensions to Understand

Take a moment to explore these in particular so you know what they do:

* **Turbo Console Log** (`chakrounanas.turbo-console-log`): Quick shortcut to auto-generate console.log statements with variable names and context.
* **Better Comments** (`aaron-bond.better-comments`): Highlights comments by type (e.g. TODO, !, ?, \*) in different colours.
* **GitLens** (`eamodio.gitlens`): Adds Git blame, commit history, and inline annotations.
* **Prettier** (`esbenp.prettier-vscode`): Auto-formats code on save for consistent styling.
* **Error Lens** (`usernamehw.errorlens`): Highlights errors and warnings inline instead of in a separate panel.
* **Todo Tree** (`gruntfuggly.todo-tree`): Extracts all TODO comments into a neat sidebar view.
* **Custom CSS Loader** (`be5invis.vscode-custom-css`): Lets you apply your own custom styling, like neon glow.

---

## 4. ⚙️ Key Editor Settings

To apply these settings:

* Go to: `Settings` (gear icon bottom left) > `Settings`
* Use the **search bar** or open **Settings (JSON)** via the Command Palette: `Cmd + Shift + P` → `Preferences: Open Settings (JSON)`
* Paste or match the settings below:

```json
{
  "workbench.colorTheme": "SynthWave '84 Min Darker Theme",
  "workbench.iconTheme": "catppuccin-frappe",
  "workbench.productIconTheme": "a-file-icon-vscode-product-icon-theme",
  "editor.wordWrap": "on",
  "files.autoSave": "onFocusChange",
  "editor.formatOnSave": true,
  "editor.minimap.autohide": true,
  "editor.cursorBlinking": "expand",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorStyle": "block-outline",
  "editor.smoothScrolling": true,
  "terminal.integrated.fontLigatures.enabled": true,
  "editor.renderWhitespace": "boundary",
  "editor.fontLigatures": true,
  "editor.guides.bracketPairs": true,
  "workbench.editor.showTabs": "single",
  "workbench.sideBar.location": "right",
  "explorer.confirmDelete": false
}
```

---

## 5. 💡 Optional - Neon Glow Effect (For SynthWave Theme)

If you want glowing text in the editor:

1. Install the extension: `be5invis.vscode-custom-css`
2. Create a `.css` file (e.g., `synthwave-glow.css`) with this content:

```css
:root {
  --synthwave-glow: 0 0 5px #f5f, 0 0 10px #f0f, 0 0 20px #f0f, 0 0 40px #f0f;
}

.monaco-editor .token {
  text-shadow: var(--synthwave-glow);
}
```

3. Open Command Palette → `Enable Custom CSS and JS`
4. Point to your `.css` file when prompted
5. Restart VS Code and allow custom styling if prompted

---

That’s it. Go one step at a time and explore what each part does.

– Brad
