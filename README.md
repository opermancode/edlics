# Edlics

Web-based file browser and code editor for Linux servers. Browse files, edit code with syntax highlighting, all from your browser.

## Quick start

```bash
npx edlics serve --hostname 0.0.0.0 --port 5000
```

Then open `http://localhost:5000` in your browser.

## Install

**Option 1 — Run on demand (no install):**
```bash
npx edlics serve --hostname 0.0.0.0 --port 5000
```

**Option 2 — Global install with npm:**
```bash
npm install -g edlics
edlics serve --hostname 0.0.0.0 --port 5000
```

**Option 3 — From source:**
```bash
git clone <repo-url>
cd edlics
npm install
sudo bash install.sh
edlics serve --hostname 0.0.0.0 --port 5000
```

## Usage

```
edlics serve [options]

Options:
  --hostname   Host to bind to (default: 127.0.0.1)
  --port       Port to listen on (default: 3000)

Examples:
  edlics serve
  edlics serve --hostname 0.0.0.0 --port 5000
```

## Features

- Flat file tree with directory navigation
- CodeMirror 6 editor with syntax highlighting
- Create, rename, delete files and folders
- Search files
- Dark theme
- No database — works directly on the filesystem

## License

MIT
