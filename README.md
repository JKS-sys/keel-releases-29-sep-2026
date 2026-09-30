# Keel — downloads

A terminal for macOS, Windows and Linux that shows at a glance which commands worked and which failed.

**Latest: [Keel 0.4.1](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/tag/v0.4.1) — 30-sep-2026**

| Computer | Download |
|---|---|
| Mac with Apple silicon (M1 and later) | [Keel-0.4.1-macos-apple-silicon-30-sep-2026.dmg](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.1/Keel-0.4.1-macos-apple-silicon-30-sep-2026.dmg) |
| Mac with Intel | [Keel-0.4.1-macos-intel-30-sep-2026.dmg](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.1/Keel-0.4.1-macos-intel-30-sep-2026.dmg) |
| Windows | [Keel-0.4.1-windows-30-sep-2026.exe](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.1/Keel-0.4.1-windows-30-sep-2026.exe) |
| Linux (AppImage) | [Keel-0.4.1-linux-30-sep-2026.AppImage](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.1/Keel-0.4.1-linux-30-sep-2026.AppImage) |
| Linux (.deb, .rpm) | on the [release page](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/tag/v0.4.1) |

**Install on macOS:** drag Keel to Applications, then run once in Terminal: `xattr -cr /Applications/Keel.app`
**Windows:** SmartScreen asks once — *More info → Run anyway*.

## What's new in 0.4.1

- **Colour everywhere, no pink:** plain output is coloured for you — numbers, paths, quoted text, links, `key=value`, errors and warnings — and brackets are coloured by depth so pairs match at a glance. What you type in zsh is coloured too: real commands gold, unknown ones red, flags, strings and paths each their own colour. Every tab has its own colour, carried along the top of its panes.
- **Open scripts with Keel:** right-click a `.command` or `.sh` file → Open With → Keel, and it runs in a new tab in its own folder. Folders open a tab there.
- **Drag files in:** drop a file on the terminal and its path is typed at the cursor, quoted if it has spaces.
- **One About section** with the app, its release notes and the creator.
- **More terminal comforts:** find with case, whole-word and regex; clickable links; copy on select; Option as Meta; ⌥←/⌥→ word jumps; ⌘⌫ clears the line; visual bell; Save Output to Downloads; Open Current Folder; Reset; Scroll to top/bottom; tabs come back next time; a question before closing something still running.
- **Releases fixed:** a home folder with spaces in its name no longer produces an empty version; every release checks the version online and carries its number, date and notes.

## Features

- **See at a glance what worked.** A gold dot beside every command that succeeded, a red ✕ beside every failure, with the exit code and time — in the gutter, on the scrollbar, on the tab and in the status bar.
- **Tabs, splits and windows** — drag a tab out for its own window, drag another tab onto the terminal to join it as a split, move a pane back to a tab, merge all windows, resize splits by dragging.
- **Open scripts with Keel** — right-click a `.command` or `.sh` file → Open With → Keel, and it runs in a new tab in its own folder. Folders open a tab there.
- **Drag files in** — drop a file or folder on the terminal and its path is typed where your cursor is, quoted if it has spaces.
- **Click to move the cursor** inside the command you are typing.
- **One About section** with the app, its release notes for every version, and the creator.
- **Everyday terminal comforts** — find with case, whole-word and regex; clickable links; copy on select; Option as Meta; ⌥←/⌥→ word jumps and ⌘⌫ to clear the line; visual bell; save the output to Downloads; open the current folder; reset; scroll to top or bottom; your tabs and folders come back next time; a question before closing something still running.
- **AI like Copilot for the command line** (Keel Pro) — suggestions as you type, ask for a command in plain words, explain a command or error, fix a failed command. Use a free offline model that Keel downloads and runs on your computer, or any AI you add by its URL.
- **Colour everywhere, no pink** — plain output is coloured for you (numbers, paths, strings, links, errors, `key=value`), brackets by depth so pairs match, what you type in zsh by meaning (real commands gold, unknown ones red), and every tab in its own colour. Colours come from the app icon: gold, warm white, warm black; light and dark themes can follow your system.
- **Small** — about 3 MB on macOS; no browser engine bundled.
- **Keel Pro** — ₹20 a month or ₹220 a year, or an activation code (needs the internet once).
- **Updates itself**, checking every download twice before installing it.

---
Made by Jagadeesh Kumar S, creator · [NewsCraft Studio on YouTube](https://www.youtube.com/@JKS-sys)