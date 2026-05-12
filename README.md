<p align="center">
  <img src="brand/logo.svg" width="80" height="80" alt="Edlics">
</p>

<h1 align="center">Edlics</h1>

<p align="center">
  <strong>Web-based code editor for Linux servers</strong>
  <br>
  Browse, edit, and manage files — right from your browser.
</p>

<p align="center">
  <a href="#quick-start"><img src="https://img.shields.io/badge/Quick_Start-blue?style=flat-square" alt="Quick Start"></a>
  <a href="#install"><img src="https://img.shields.io/badge/Install-green?style=flat-square" alt="Install"></a>
  <a href="#usage"><img src="https://img.shields.io/badge/Usage-purple?style=flat-square" alt="Usage"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-white?style=flat-square" alt="License"></a>
</p>

<br>

## Quick start

```bash
npx edlics serve --hostname 0.0.0.0 --port 5000
```

Open `http://localhost:5000` in your browser.

<br>

## Install

### Run on demand (no install)

```bash
npx edlics serve
```

### Global install via npm

```bash
npm install -g edlics
edlics serve --hostname 0.0.0.0 --port 5000
```

### From source

```bash
git clone https://github.com/your-username/edlics.git
cd edlics
npm install
sudo bash install.sh
edlics serve --hostname 0.0.0.0 --port 5000
```

<br>

## Features

| | |
|---|---|
| **File browser** | Flat file tree with directory navigation, hidden file dimming, search |
| **Code editor** | CodeMirror 6 with syntax highlighting for JS, TS, Python, HTML, CSS, JSON, Markdown, XML, YAML |
| **File operations** | Create, rename, delete files and folders — right-click context menu |
| **Dark theme** | Easy on the eyes, works day and night |
| **No database** | Works directly on the filesystem — what you see is what's on disk |
| **Async by design** | Non-blocking file I/O, handles large files without hiccups |

<br>

## Usage

```text
edlics serve [options]

Options:
  --hostname   Host to bind to (default: 127.0.0.1)
  --port       Port to listen on (default: 3000)

Examples:
  edlics serve
  edlics serve --hostname 0.0.0.0 --port 5000
```

<br>

## Keyboard shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+S` | Save file |
| `Ctrl+P` | Search files |
| `Ctrl+W` | Close tab |
| `F2` | Rename file |
| `Escape` | Close dialogs / menus |

<br>

## Screenshots

> _(Add a screenshot here once you've launched it)_

<br>

## Project structure

```text
edlics/
├── bin/
│   └── edlics.js          # HTTP server + file API (Node.js)
├── bundle/
│   └── editor.mjs         # CodeMirror 6 build entry point
├── public/
│   ├── editor.mjs         # Pre-built editor bundle
│   └── index.html         # Single-page frontend
├── .gitignore
├── README.md
├── install.sh             # Symlinks edlics to /usr/local/bin
└── package.json           # Dependencies + build scripts
```

<br>

## Tech stack

- **Frontend:** Vanilla JS, CodeMirror 6, CSS custom properties
- **Backend:** Node.js (no frameworks — bare `http` module)
- **Editor:** CodeMirror 6 with syntax highlighting, bracket matching, undo history
- **Theme:** One Dark (Atom-inspired dark theme)

<br>

## License

MIT — use it, share it, build on it.
