<div align="center">
  <h1 style="color:#f0f">🧑‍💻 Brad's VS Code Setup Guide</h1>
  <p>This guide walks you through replicating my full Visual Studio Code setup, including themes, icons, extensions, and custom settings.</p>
  <strong>No syncing. No scripts. Just clean manual setup.</strong>
</div>



⸻

🎨 Theme and Icon Setup

🎨 Color Theme
	•	SynthWave ’84 Min Darker Theme
🔍 Search: fernaandojr.synthwave-remix-min-darker
⚙️ Apply: Settings > Theme > Color Theme

🗂 File Icon Theme
	•	Catppuccin Frappé Icons
🔍 Search: catppuccin.catppuccin-vsc-icons
⚙️ Apply: Settings > Theme > File Icon Theme

🧩 Product Icon Theme
	•	Atom Material Product Icons
🔍 Search: atommaterial.a-file-icon-vscode
⚙️ Apply: Settings > Theme > Product Icon Theme

⸻

🔌 Extensions to Install

Use the Extensions sidebar (⇧⌘X) and search for each of the following:

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

✨ Key Extensions to Explore

💡 These add superpowers — take a minute to understand what they do:
	•	⚡ Turbo Console Log: Auto-generates console.log() with context
	•	🟡 Better Comments: Colour-coded comment tags like // TODO: or // ! warning
	•	🔍 GitLens: Git blame, authorship, commit history — right inside VS Code
	•	🧼 Prettier: Auto-formats your code cleanly when you save
	•	❗ Error Lens: Puts errors and warnings inline for fast debugging
	•	📌 Todo Tree: Pulls all your TODOs into one easy sidebar
	•	🎨 Custom CSS Loader: Lets you use themes like SynthWave with neon glow

⸻

⚙️ Key Editor Settings

To apply these:
	•	Open Settings (gear icon bottom left)
	•	Or use Command Palette → Preferences: Open Settings (JSON)

Then paste:

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

💡 Neon Glow Effect (Optional)

Want glowing text like the SynthWave demo screenshots?
	1.	Install be5invis.vscode-custom-css
	2.	Create a .css file (like synthwave-glow.css) with:

:root {
  --synthwave-glow: 0 0 5px #f5f, 0 0 10px #f0f, 0 0 20px #f0f, 0 0 40px #f0f;
}

.monaco-editor .token {
  text-shadow: var(--synthwave-glow);
}

	3.	Command Palette → Enable Custom CSS and JS
	4.	Select your .css file when prompted
	5.	Restart VS Code and click “Allow” if prompted

⸻


<div align="center">
  <strong>That's it!</strong><br>
  Go step by step, enjoy your custom editor, and explore how each piece works.
  <br><br>
  — Brad
</div>
