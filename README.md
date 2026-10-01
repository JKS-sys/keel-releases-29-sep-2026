<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/keel-icon-dark.png">
    <img src="assets/keel-icon-light.png" width="128" height="128" alt="Keel app icon: a gold >_ prompt on a rounded square">
  </picture>
</p>

# Keel — downloads

A terminal for macOS, Windows and Linux that shows at a glance which commands worked and which failed.

**Latest: [Keel 0.4.2](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/tag/v0.4.2) — 01-oct-2026**

| Computer | Download |
|---|---|
| Mac with Apple silicon (M1 and later) | [Keel-0.4.2-macos-apple-silicon-01-oct-2026.dmg](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.2/Keel-0.4.2-macos-apple-silicon-01-oct-2026.dmg) |
| Mac with Intel | [Keel-0.4.2-macos-intel-01-oct-2026.dmg](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.2/Keel-0.4.2-macos-intel-01-oct-2026.dmg) |
| Windows | [Keel-0.4.2-windows-01-oct-2026.exe](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.2/Keel-0.4.2-windows-01-oct-2026.exe) |
| Linux (AppImage) | [Keel-0.4.2-linux-01-oct-2026.AppImage](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.2/Keel-0.4.2-linux-01-oct-2026.AppImage) |
| Linux (.deb, .rpm) | on the [release page](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/tag/v0.4.2) |

**Install on macOS:** drag Keel to Applications, then run once in Terminal: `xattr -cr /Applications/Keel.app`
**Windows:** SmartScreen asks once — *More info → Run anyway*.

## What's new in 0.4.2

- **`.command` files run when opened with Keel.** Keel now waits for the shell's first prompt before typing the script (it used to be typed too early and swallowed, leaving an empty tab), picks up files macOS hands over while Keel is still starting, and runs scripts that lost their execute bit through their `#!` line.
- **Folders open with Keel:** right-click a folder → Open With → Keel (on Windows, “Open in Keel”) for a new tab in that folder.
- **Window names in the Dock:** right-clicking Keel in the Dock lists each window by its tab and folder, not “Keel” for all of them.
- **Animated tab icons** for what each tab is doing — building, downloading, testing, serving, SSH, git, editing, scripts and more — each in its own colour, never pink.
- **A new failure badge** in place of the red ✕: its colour and mark say why — error, command not found, not allowed, wrong usage, stopped with Ctrl-C, crashed.
- **Sounds and animation:** a chime when a command works, a low tone when it fails, ticks for tabs; Settings → Sounds and Motion.
- **About fits on one screen:** two columns; only the newest release notes are open, older versions are one click away.
- **Colour everywhere, no pink:** plain output is coloured for you — numbers, paths, quoted text, links, `key=value`, errors and warnings — and brackets are coloured by depth so pairs match at a glance. What you type in zsh is coloured too: real commands gold, unknown ones red, flags, strings and paths each their own colour. Every tab has its own colour, carried along the top of its panes.
- **Open scripts with Keel:** right-click a `.command` or `.sh` file → Open With → Keel, and it runs in a new tab in its own folder. Folders open a tab there.
- **Drag files in:** drop a file on the terminal and its path is typed at the cursor, quoted if it has spaces.
- **One About section** with the app, its release notes and the creator.
- **More terminal comforts:** find with case, whole-word and regex; clickable links; copy on select; Option as Meta; ⌥←/⌥→ word jumps; ⌘⌫ clears the line; visual bell; Save Output to Downloads; Open Current Folder; Reset; Scroll to top/bottom; tabs come back next time; a question before closing something still running.
- **Releases fixed:** a home folder with spaces in its name no longer produces an empty version; every release checks the version online and carries its number, date and notes.

## Features

- **See at a glance what worked.** A gold check beside every command that succeeded and a failure badge whose colour and mark say why — a cross for an error, ? for “command not found”, a barred circle for “not allowed”, a square for Ctrl-C — with the exit code and time, in the gutter, on the scrollbar, on the tab and in the status bar.
- **Animated tab icons** — each tab shows what it is doing: building, downloading, uploading, testing, serving, editing, git, SSH, sudo, AI or a script, each in its own colour (never pink).
- **Sounds and motion** — a soft chime when a command works, a low tone when it fails, ticks for new and closed tabs; choose off, failures and long commands, or every command. Tabs, marks and panels animate; Reduce motion turns it all off.
- **Tabs, splits and windows** — drag a tab out for its own window, drag another tab onto the terminal to join it as a split, move a pane back to a tab, merge all windows, resize splits by dragging.
- **Open scripts and folders with Keel** — right-click a `.command` or `.sh` file → Open With → Keel and it runs in a new tab in its own folder, once the shell is ready (scripts without the execute bit run through their `#!` line). Right-click a folder → Open With → Keel (Windows: “Open in Keel”) for a tab already in that folder.
- **Windows named by what they hold** — the Dock's right-click menu and the Window menu list each window by its tab and folder.
- **Drag files in** — drop a file or folder on the terminal and its path is typed where your cursor is, quoted if it has spaces.
- **Click to move the cursor** inside the command you are typing.
- **One About section** with the app, its release notes for every version (newest open, older ones one click away, so it fits without scrolling), and the creator.
- **Everyday terminal comforts** — find with case, whole-word and regex; clickable links; copy on select; Option as Meta; ⌥←/⌥→ word jumps and ⌘⌫ to clear the line; visual bell; save the output to Downloads; open the current folder; reset; scroll to top or bottom; your tabs and folders come back next time; a question before closing something still running.
- **AI like Copilot for the command line** (Keel Pro) — suggestions as you type, ask for a command in plain words, explain a command or error, fix a failed command. Use a free offline model that Keel downloads and runs on your computer, or any AI you add by its URL.
- **Colour everywhere, no pink** — plain output is coloured for you (numbers, paths, strings, links, errors, `key=value`), brackets by depth so pairs match, what you type in zsh by meaning (real commands gold, unknown ones red), and every tab in its own colour. Colours come from the app icon: gold, warm white, warm black; light and dark themes can follow your system.
- **Small** — about 3 MB on macOS; no browser engine bundled.
- **Keel Pro** — ₹20 a month or ₹220 a year, or an activation code (needs the internet once).
- **Updates itself**, checking every download twice before installing it.

---
Made by Jagadeesh Kumar S, creator · [NewsCraft Studio on YouTube](https://www.youtube.com/@JKS-sys)