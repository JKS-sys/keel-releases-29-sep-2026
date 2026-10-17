<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/keel-icon-dark.png">
    <img src="assets/keel-icon-light.png" width="128" height="128" alt="Keel app icon: a gold >_ prompt on a rounded square">
  </picture>
</p>
<p align="center">
  <img src="assets/keel-icon-light.png" width="48" height="48" alt="Keel icon, light"> &nbsp; <img src="assets/keel-icon-dark.png" width="48" height="48" alt="Keel icon, dark">
</p>

# Keel — AI Terminal

An AI terminal for macOS, Windows, Linux, ChromeOS and FreeBSD that shows at a glance which commands worked and which failed, with offline AI that is free for everyone.

> ⭐ **If Keel helps you, please give this repository a star** — [★ Star on GitHub](https://github.com/JKS-sys/keel-releases-29-sep-2026) — it is how other people find it, and it tells me what to build next.

**Website:** [ipconfig.co.network](https://ipconfig.co.network) · **App page:** [ipconfig.co.network/keel](https://ipconfig.co.network/keel) · **Releases:** [github.com/JKS-sys/keel-releases-29-sep-2026/releases](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases)

**Latest: [Keel 0.4.7](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/tag/v0.4.7) — 17-oct-2026** · [release notes](https://ipconfig.co.network/updates/keel/release-notes-0.4.7.md)

## Install

**macOS, Linux, ChromeOS and FreeBSD — with [Pour](https://ipconfig.co.network/pour), in two commands:**

```sh
curl -fsSL https://ipconfig.co.network/pour/install | sh
pour install --cask keel
```

**Windows — with Pour:** download [pour-windows-x86_64.exe](https://ipconfig.co.network/pour/dl/pour-windows-x86_64.exe), then in PowerShell:

```powershell
.\pour-windows-x86_64.exe install --cask keel
```

Pour picks the right installer for your computer, checks its SHA-256 against `latest.json` and keeps Keel up to date with `pour upgrade`.

**Or download it yourself:**

- **macOS** — [Apple silicon](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-macos-apple-silicon-17-oct-2026.dmg) · [Intel](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-macos-intel-17-oct-2026.dmg): drag Keel to Applications, then run once in Terminal: `xattr -cr /Applications/Keel.app`.
- **Windows 10 and 11** — [x64](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-windows-x64-17-oct-2026.exe) · [ARM64](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-windows-arm64-17-oct-2026.exe). SmartScreen asks once — *More info → Run anyway*.
- **Linux** — [.deb x86_64](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-linux-amd64-17-oct-2026.deb) · [.deb ARM64](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-linux-arm64-17-oct-2026.deb) · [.rpm x86_64](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-linux-x86_64-17-oct-2026.rpm) · [.rpm ARM64](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-linux-aarch64-17-oct-2026.rpm) · [AppImage x86_64](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-linux-x86_64-17-oct-2026.AppImage) (`chmod +x`, then run it).
- **ChromeOS** — turn on *Settings → About ChromeOS → Developers → Linux development environment*, then install the Linux .deb for your Chromebook (`sudo apt install ./Keel-…deb`), or use Pour in the Linux terminal.
- **FreeBSD 14** — [x86_64 tarball](https://github.com/JKS-sys/keel-releases-29-sep-2026/releases/download/v0.4.7/Keel-0.4.7-freebsd-x86_64-17-oct-2026.tar.gz): `sudo pkg install gtk3 webkit2-gtk_41 libsoup3`, unpack, run `./keel`.
- **Haiku** — not available: the web view library Keel is built on has no Haiku backend yet, so there is no honest way to ship it there.

**No Pour, one line (macOS and Linux):** `curl -fsSL https://ipconfig.co.network/updates/keel/install.sh | bash`

Keel updates itself: every launch checks `https://ipconfig.co.network/updates/keel/latest.json` (and the GitHub releases as a second source), and an update installs from the status bar.

## See it move

Each animation plays right here; click one for the full-quality video with sound.

### The start-up

<a href="assets/demos/startup.mp4"><img src="assets/demos/startup.webp" width="900" alt="Keel — The start-up (animation; click for the video with sound)"></a>

The tile draws itself, sparks fly, "Keel" rises, "An AI terminal" types itself and "By Jagadeesh Kumar S" fades in — then straight to your shell. Any key skips it. · [▶ video with sound](assets/demos/startup.mp4)

### Every command marked, every word coloured

<a href="assets/demos/marks.mp4"><img src="assets/demos/marks.webp" width="900" alt="Keel — Every command marked, every word coloured (animation; click for the video with sound)"></a>

A gold check for a command that worked, a red badge that says why for one that failed — in the gutter, on the scrollbar, on the tab and in the status bar. Numbers, paths, strings, versions and brackets each get their own colour, with no pink anywhere. · [▶ video with sound](assets/demos/marks.mp4)

### Ask for a command

<a href="assets/demos/ai-ask.mp4"><img src="assets/demos/ai-ask.webp" width="900" alt="Keel — Ask for a command (animation; click for the video with sound)"></a>

⌘I (or `# …` at the prompt): describe what you want in plain words and get one exact command back. Nothing runs until you choose Run. · [▶ video with sound](assets/demos/ai-ask.mp4)

### Fix a failed command

<a href="assets/demos/ai-fix.mp4"><img src="assets/demos/ai-fix.webp" width="900" alt="Keel — Fix a failed command (animation; click for the video with sound)"></a>

A command failed: Fix with AI reads the error and suggests the fix. Offline models on your own computer are free for everyone. · [▶ video with sound](assets/demos/ai-fix.mp4)

### Tabs, splits and arranging

<a href="assets/demos/splits.mp4"><img src="assets/demos/splits.webp" width="900" alt="Keel — Tabs, splits and arranging (animation; click for the video with sound)"></a>

Split right and down, then Arrange → Grid, Columns or Rows lays every pane out in one click. Each tab keeps its own colour. · [▶ video with sound](assets/demos/splits.mp4)

### Right-click menus

<a href="assets/demos/menus.mp4"><img src="assets/demos/menus.webp" width="900" alt="Keel — Right-click menus (animation; click for the video with sound)"></a>

Right-click anywhere for a menu that fits what is under the pointer: submenus for Look, Arrange and AI, checkmarks, keyboard shortcuts — and in a small window the menu becomes a drill-down list so nothing is cut off. · [▶ video with sound](assets/demos/menus.mp4)

### The menu-bar quick panel

<a href="assets/demos/quick-panel.mp4"><img src="assets/demos/quick-panel.webp" width="900" alt="Keel — The menu-bar quick panel (animation; click for the video with sound)"></a>

Click Keel’s icon in the menu bar: open windows, recent folders, twelve one-click actions and where Keel lives (Dock, menu bar, both or in the background). · [▶ video with sound](assets/demos/quick-panel.mp4)

### Settings

<a href="assets/demos/settings.mp4"><img src="assets/demos/settings.webp" width="900" alt="Keel — Settings (animation; click for the video with sound)"></a>

Ten pages on an icon rail: Look, Sound & Motion (with every sound and its animation), Terminal, Notifications, Menus & Dock, Account, AI, Keel Pro, Privacy and Updates. · [▶ video with sound](assets/demos/settings.mp4)

### Sign in with an email code

<a href="assets/demos/account.mp4"><img src="assets/demos/account.webp" width="900" alt="Keel — Sign in with an email code (animation; click for the video with sound)"></a>

One account for every ipconfig app: type your email, then the 6-digit code — Keel signs in by itself. Your computers, seats and subscriptions, all in one place. · [▶ video with sound](assets/demos/account.mp4)

### The Owner Panel

<a href="assets/demos/owner.mp4"><img src="assets/demos/owner.webp" width="900" alt="Keel — The Owner Panel (animation; click for the video with sound)"></a>

Always connected to the dashboard: installs, people, codes, subscriptions and crash reports with search, bulk actions and eight layouts — list, cards, compact, tiles, board, timeline, magazine and masonry. · [▶ video with sound](assets/demos/owner.mp4)

### Small windows stay tidy

<a href="assets/demos/small-window.mp4"><img src="assets/demos/small-window.webp" width="900" alt="Keel — Small windows stay tidy (animation; click for the video with sound)"></a>

Shrink the window and nothing overlaps or scrolls sideways: the toolbar wraps, Settings folds its rail into icons, and the terminal reflows. · [▶ video with sound](assets/demos/small-window.mp4)

## Screenshots

<img src="assets/screenshots/shot-terminal.webp" width="900" alt="Keel — The terminal: gold checks for commands that worked, a red badge for the one that failed, and every kind of output in its own colour — branches, paths, versions, times, ok and failed.">

*The terminal: gold checks for commands that worked, a red badge for the one that failed, and every kind of output in its own colour — branches, paths, versions, times, ok and failed.*

<img src="assets/screenshots/shot-ai-ask.webp" width="900" alt="Keel — Ask for a command: the AI card waits at the bottom right while the terminal stays usable.">

*Ask for a command: the AI card waits at the bottom right while the terminal stays usable.*

<img src="assets/screenshots/shot-ai-fix.webp" width="900" alt="Keel — A command failed: Fix with AI suggests the corrected command with Insert, Run and Copy.">

*A command failed: Fix with AI suggests the corrected command with Insert, Run and Copy.*

<img src="assets/screenshots/shot-splits.webp" width="900" alt="Keel — Four panes arranged in a grid, each its own shell, the active one outlined in gold.">

*Four panes arranged in a grid, each its own shell, the active one outlined in gold.*

<img src="assets/screenshots/shot-menu.webp" width="900" alt="Keel — The right-click menu with its Arrange submenu open: Grid, Columns, Rows and Main + side.">

*The right-click menu with its Arrange submenu open: Grid, Columns, Rows and Main + side.*

<img src="assets/screenshots/shot-quick.webp" width="900" alt="Keel — The menu-bar quick panel: windows, recent folders, twelve actions and where Keel lives.">

*The menu-bar quick panel: windows, recent folders, twelve actions and where Keel lives.*

<img src="assets/screenshots/shot-settings-look.webp" width="900" alt="Keel — Settings → Look: themes, transparency, text size and the colours of your output.">

*Settings → Look: themes, transparency, text size and the colours of your output.*

<img src="assets/screenshots/shot-settings-sound.webp" width="900" alt="Keel — Settings → Sound & Motion: Off, Subtle or Lively, thirteen sound sets, and every sound with the animation it plays.">

*Settings → Sound & Motion: Off, Subtle or Lively, thirteen sound sets, and every sound with the animation it plays.*

<img src="assets/screenshots/shot-settings-menus.webp" width="900" alt="Keel — Settings → Menus & Dock: where Keel lives (Dock, menu bar, both or background), right-click menus in Finder, Explorer and Linux file managers.">

*Settings → Menus & Dock: where Keel lives (Dock, menu bar, both or background), right-click menus in Finder, Explorer and Linux file managers.*

<img src="assets/screenshots/shot-account.webp" width="900" alt="Keel — Settings → Account: signed in, Keel Pro, the seats in use, your computers and subscriptions.">

*Settings → Account: signed in, Keel Pro, the seats in use, your computers and subscriptions.*

<img src="assets/screenshots/shot-owner.webp" width="900" alt="Keel — The Owner Panel overview: installs, active computers, Pro, revenue, codes and crash reports, connected to the dashboard.">

*The Owner Panel overview: installs, active computers, Pro, revenue, codes and crash reports, connected to the dashboard.*

<img src="assets/screenshots/shot-owner-cards.webp" width="900" alt="Keel — The Owner Panel’s install list in the cards layout, one of eight.">

*The Owner Panel’s install list in the cards layout, one of eight.*

<img src="assets/screenshots/shot-light.webp" width="900" alt="Keel — The light theme: the same colours, tuned for a bright screen.">

*The light theme: the same colours, tuned for a bright screen.*

<img src="assets/screenshots/shot-small.webp" width="900" alt="Keel — A small window (560 × 380): nothing overlaps and nothing scrolls sideways.">

*A small window (560 × 380): nothing overlaps and nothing scrolls sideways.*

<img src="assets/screenshots/mac-split.webp" width="900" alt="Keel — Keel on the Mac: two panes side by side, each its own shell, the active one marked in gold.">

*Keel on the Mac: two panes side by side, each its own shell, the active one marked in gold.*

<img src="assets/screenshots/mac-light.webp" width="900" alt="Keel — The light theme on the Mac, two tabs, every tab in its own colour.">

*The light theme on the Mac, two tabs, every tab in its own colour.*

<img src="assets/screenshots/mac-dark.webp" width="900" alt="Keel — The dark theme on the Mac: warm black, gold and warm white, straight from the app icon.">

*The dark theme on the Mac: warm black, gold and warm white, straight from the app icon.*

## What's new in 0.4.7

- **Every system, built on your Mac.** `bash update.sh` now builds every installer itself — macOS (Apple silicon and Intel), Windows x64 and ARM64 (cross-compiled), Linux x86_64 and ARM64 (.deb, .rpm, AppImage, in Docker), FreeBSD 14 — side by side with a live board, no GitHub Actions. ChromeOS installs the Linux .deb. Haiku is not possible (no web view backend), and the notes say so.
- **Install with Pour** on every system: `pour install --cask keel`. Keel registers itself on Pour at every release; no Homebrew tap any more.
- **Mac App Store and Microsoft Store** packages are built and submitted automatically once `.env` has their credentials (left empty for now).
- **Accounts.** Sign in with an emailed 6-digit code or a password, one account for every ipconfig app; Pro follows your account to two computers, with "Use this computer instead", your devices and subscriptions in Settings → Account, and 14 days offline.
- **The Owner Panel is always connected** to the ipconfig dashboard — no connect or sync button: installs, people, devices, codes, subscriptions and crash reports with search, bulk actions, export and eight layouts.
- **Menu bar, Dock and background.** Keel can live in the Dock, the menu bar, both, or in the background (and the background process can be turned off). The menu-bar icon opens a quick panel on a left click and a full menu on a right click; the Dock icon's right-click menu has New Window, New Tab, a folder, a script, AI, the speed test, recent folders and more. While Keel is in the Dock, closing the last window or tab quits it completely.
- **Right-click in Finder, Explorer and Linux file managers:** New Keel Tab / Window Here, Split Here, Run, Edit, Git Status, Folder Size, List Files, Ask AI, Copy Path.
- **Desktop notifications** for long or failed commands, updates and Pro — click one and the very window it came from comes back.
- **`speed`** now shows download **and upload** speed and latency (`curl -fsSL https://ipconfig.co.network/speed | sh`), in zsh, bash, fish and PowerShell.
- **Richer right-click menus** with submenus, checkmarks and shortcuts; Arrange Panes as a grid, columns, rows or main + side; menus become drill-down lists in small windows.
- **More colour, no pink:** TODOs, ✓ and ✗, `code`, **bold**, table borders and separator lines, nine tab colours.
- **More sound and motion:** 44 sounds in 13 sets, each with its own vector animation; Motion Off, Subtle or Lively.
- **Settings in ten pages** on an icon rail; small windows never overlap or scroll sideways.
- **README:** eleven animated demos (with sound in the videos) and fourteen 2× screenshots, recorded from the real interface; a star request at the top and the end; all 20 GitHub topics.
- Keel is now under a proprietary licence (LICENSE).

## Features

- **See at a glance what worked.** A gold check beside every command that succeeded and a failure badge whose colour and mark say why — a cross for an error, ? for “command not found”, a barred circle for “not allowed”, a square for Ctrl-C — with the exit code and time, in the gutter, on the scrollbar, on the tab and in the status bar.
- **Offline AI, free for everyone.** Install a model in Settings → AI (a catalogue of 20, from 400 MB up, marked by what fits this computer's memory), or use any GGUF file, folder, Hugging Face link, or an AI app already running here — Ollama, LM Studio, Jan, GPT4All, llama.cpp, LocalAI, vLLM, text-generation-webui, llamafile. Nothing leaves your computer.
- **Ask, Explain, Fix, autocomplete.** Type `# what you want` at the prompt or press ⌘I for one exact command; ⇧⌘E explains; ⇧⌘F fixes a failed command; grey suggestions as you type come from your history, exact completions, then the AI.
- **GitHub Copilot and AI services by URL** (Keel Pro) — OpenAI, Gemini, Groq, Mistral, DeepSeek, OpenRouter or any OpenAI-compatible server.
- **One account for every ipconfig app** — sign in with an emailed 6-digit code (it signs in by itself at the sixth digit) or a password; Pro follows your account to up to two computers, with “Use this computer instead” when every seat is taken, your subscriptions and devices in Settings → Account, and 14 days offline.
- **Lives where you want** — in the Dock, in the menu bar, both, or in the background (Settings → Menus & Dock). While Keel is in the Dock, closing the last window or tab quits it completely.
- **Menu-bar icon** — left click opens a quick panel (windows, recent folders, twelve one-click actions, where Keel lives); right click opens the full menu.
- **Dock menu** — right-click Keel in the Dock: New Window, New Tab, a tab in a folder, run a script, Ask AI, Fix, Speed Test, Quick Panel, Gather or Merge windows, Recent Folders, Keel Lives In and More.
- **Right-click in Finder, Explorer and Linux file managers** — on files and folders: New Keel Tab / Window Here, Split Here, Run in Keel, Edit in Keel, Git Status, Folder Size, List Files, Ask AI About It, Copy Path (macOS Services, a Windows “Keel” submenu, Nautilus, Caja, Nemo and Dolphin).
- **Desktop notifications** — when a long command finishes or fails while you are elsewhere, when an update is ready, when Pro changes; clicking one brings back the very window it came from.
- **Right-click menus everywhere** — terminal, tabs, marks, links, folders — with submenus, checkmarks and shortcuts; in a small window they turn into a list you drill into.
- **Tabs, splits and windows** — drag a tab out for its own window or onto a terminal to join it as a split; Arrange Panes as a grid, columns, rows or main + side; merge all windows; resize by dragging. Small windows never overlap or scroll sideways.
- **Colour everywhere, no pink** — plain output is coloured for you (numbers, paths, strings, links, errors, versions, dates, sizes, durations, TODOs, ✓ and ✗, `code`, **bold**, table borders), brackets by depth so pairs match, every tab in its own colour, nine tab hues. Light and dark themes follow your system.
- **Animations and sounds** — 44 sounds in 13 sound sets, every one with its own self-drawing vector animation; Motion Off, Subtle or Lively, with tiny interface sounds in Lively only.
- **Start-up** — the tile draws itself, sparks fly, "Keel" rises, "An AI terminal" types itself, "By Jagadeesh Kumar S" fades in, with a synthesised chord; any key skips it.
- **Built-in `speed`** — download and upload speed and latency from ipconfig.co.network, in every shell.
- **Owner Panel** (on the owner's computer only), always connected to the ipconfig dashboard: installs, people, devices, activation codes, subscriptions and crash reports — search, bulk actions, export, and eight layouts.
- **Markets** (on the owner's computer): signals with a trade plan, out-of-sample success rates and confidence grades — honest numbers, never a promise.
- **Crash reports** — written to `~/.keel/crashes`; sent only with a yes, and never with a command, output or file name of yours.
- **Every system** — macOS (Apple silicon and Intel), Windows 10/11 (x64 and ARM64), Linux (x86_64 and ARM64: .deb, .rpm, AppImage), ChromeOS (through its Linux environment) and FreeBSD 14.
- **Keel Pro** — ₹20 a month or ₹220 a year, or an activation code. The terminal, the marks and the offline AI are free for good.
- **Updates itself**, checking every download twice (SHA-256 and an Ed25519 signature) before installing it.

---

> ⭐ **If Keel helps you, please give this repository a star** — [★ Star on GitHub](https://github.com/JKS-sys/keel-releases-29-sep-2026) — it is how other people find it, and it tells me what to build next.

Made by Jagadeesh Kumar S, creator · [NewsCraft Studio on YouTube](https://www.youtube.com/@JKS-sys) · [ipconfig.co.network](https://ipconfig.co.network) · Licence: see [LICENSE](LICENSE)