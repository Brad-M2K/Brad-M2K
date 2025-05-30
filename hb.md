🧑‍💻 Brad’s VS Code Setup Guide

This guide walks you through replicating my full Visual Studio Code setup, including themes, icons, extensions, and custom settings.

No syncing. No scripts. Just clean manual setup.

⸻

🎨 1. Theme and Icon Setup

🎨 Color Theme

SynthWave ’84 Min Darker Theme
🔍 Search: fernaandojr.synthwave-remix-min-darker
⚙️ Apply: Settings > Theme > Color Theme

🗂 File Icon Theme

Catppuccin Frappé Icons
🔍 Search: catppuccin.catppuccin-vsc-icons
⚙️ Apply: Settings > Theme > File Icon Theme

🧩 Product Icon Theme

Atom Material Product Icons
🔍 Search: atommaterial.a-file-icon-vscode
⚙️ Apply: Settings > Theme > Product Icon Theme

⸻

🔌 2. Extensions to Install

Use the Extensions sidebar (⇧⌘X) and search for each of the following manually:

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


⸻

✨ 3. Key Extensions to Understand

These are especially useful. Take a minute to learn what they do:

⚡ Turbo Console Log

chakrounanas.turbo-console-log

Auto-generates console.log() lines with context info for quick debugging.

🟡 Better Comments

aaron-bond.better-comments

Adds colours and categories (TODO, !, ?, *) to improve readability of comments.

🔍 GitLens

eamodio.gitlens

Adds Git blame, authorship, history, and visual inline annotations.

🧼 Prettier

esbenp.prettier-vscode

Automatically formats code on save to maintain consistent style.

❗ Error Lens

usernamehw.errorlens

Displays warnings and errors inline instead of just in the Problems panel.

📌 Todo Tree

gruntfuggly.todo-tree

Finds all TODOs and FIXMEs across files and shows them in a side panel.

🎨 Custom CSS Loader

be5invis.vscode-custom-css

Lets you add custom styling to VS Code like SynthWave’s neon glow.

⸻

⚙️ 4. Key Editor Settings

To apply these:
	•	Go to Settings (gear icon) > Settings
	•	Or open via Command Palette: Cmd + Shift + P → Preferences: Open Settings (JSON)

Paste in the settings below:

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


⸻

💡 5. Optional — Neon Glow Effect (SynthWave Style)

If you want glowing text inside the editor:

Step-by-step:
	1.	Install: be5invis.vscode-custom-css
	2.	Create a file called synthwave-glow.css
	3.	Paste this:

:root {
  --synthwave-glow: 0 0 5px #f5f, 0 0 10px #f0f, 0 0 20px #f0f, 0 0 40px #f0f;
}

.monaco-editor .token {
  text-shadow: var(--synthwave-glow);
}

	4.	Open Command Palette → Enable Custom CSS and JS
	5.	Select your CSS file when prompted
	6.	Restart VS Code and approve the styling warning

⸻


<div align="center">
  <strong>That's everything!</strong><br>
  Try one section at a time and enjoy your custom setup.
  <br><br>
  — Brad
</div>
