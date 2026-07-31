# Sketchboard

A local-first drawing and annotation app that runs entirely in your browser. No server, no accounts, no installation required.

**Version:** 1.0.0  
**Released:** 2026-07-31

---

## Quick Start

1. Download `index.html` from this repository
2. Double-click it to open in any modern browser
3. Start drawing

That's it. No installation, no setup, no internet required.

---

## Installation & Deployment

### Option 1: Local file (simplest)

Download `index.html` and open it directly in your browser. Works offline.

### Option 2: Static web hosting

Upload `index.html` to any static hosting service:

| Service | How |
|---------|-----|
| **GitHub Pages** | Fork this repo, enable Pages in Settings |
| **Netlify** | Drag and drop `index.html` at app.netlify.com/drop |
| **Vercel** | Import this repo at vercel.com/new |
| **AWS S3** | Upload to an S3 bucket with static website hosting enabled |
| **Any web server** | Place `index.html` in the document root |

### Option 3: Embed in another page

```html
<iframe src="index.html" width="100%" height="600px" frameborder="0"></iframe>
```

### Option 4: Share via email/USB

The entire application is a single 2.5 MB file. Send it as an email attachment, put it on a USB drive, or share it via AirDrop/file transfer.

---

## Features

### Drawing Tools
- **Shapes**: Rectangle, Diamond, Ellipse, Line, Arrow
- **Freehand**: Pencil drawing with pressure sensitivity
- **Text**: Add text annotations anywhere
- **Images**: Paste or drag images onto the canvas

### Shadow System
- Automatic shadow applied to imported images
- Adjustable blur, offset, padding, and strength
- Presets: None, Subtle, Professional, Dramatic
- Real-time preview as you adjust

### File Operations
- **New**: Clear canvas and start fresh
- **Open**: Load `.excalidraw` files
- **Save**: Export as `.excalidraw` format
- **Export**: Download as PNG image

### Autosave
- Automatically saves to browser storage every 3 seconds after changes
- Persists across browser sessions and page refreshes
- "Saved" indicator in the top-right corner

### Keyboard Shortcuts
- `Cmd/Ctrl + S` — Save as .excalidraw file
- `1` — Selection tool
- `2` — Rectangle
- `3` — Diamond
- `4` — Ellipse
- `5` — Arrow
- `6` — Line
- `7` — Pencil
- `8` — Text
- `9` — Image
- `Cmd/Ctrl + Z` — Undo
- `Cmd/Ctrl + Shift + Z` — Redo

---

## User Manual

### Adding Images

1. Click the Image tool (icon 9) in the toolbar, or
2. Paste an image from clipboard (`Cmd/Ctrl + V`), or
3. Drag and drop an image file onto the canvas

Images automatically receive a shadow effect that can be customized.

### Customizing Shadows

1. Click on an image to select it
2. The shadow controls panel appears on the right side
3. Adjust sliders:
   - **Blur**: Shadow softness (0-100)
   - **Offset**: Distance of shadow from image (0-50)
   - **Padding**: Extra space around the image (0-80)
   - **Strength**: Shadow darkness (0-100)
4. Or click a preset button for quick styling

### Saving Your Work

- **Automatic**: Your canvas saves to browser storage automatically
- **Manual save**: Press `Cmd/Ctrl + S` to download a `.excalidraw` file
- **Export PNG**: Click `Export` > `Export as PNG` for a shareable image

### Opening Saved Files

1. Click **Open** in the menu bar
2. Select a `.excalidraw` file from your computer
3. The canvas loads with all your previous work

---

## System Requirements

- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No internet connection required
- No backend, server, or database needed
- Works on macOS, Windows, Linux, ChromeOS, iOS, Android

---

## Troubleshooting

| Problem | Solution |
|---------|----------|
| Blank page when opening file | Make sure you're using a modern browser (Chrome 90+, Firefox 88+, Safari 14+). Try right-click > "Open with" and select your browser. |
| Canvas won't save | Check browser storage isn't full. Try clearing other site data if storage is at capacity. |
| Images won't paste | Some browsers restrict clipboard access on `file://`. Try opening via a local server: `python3 -m http.server 8000` then visit `localhost:8000`. |
| Shadow controls not showing | Click directly on the image to select it. The panel appears only when an image element is selected. |
| File too large to email | The app is 2.5 MB which is within most email limits. If blocked, use a file sharing service or zip it first. |
| Lost my work after clearing browser data | Browser storage is local. Use `Cmd/Ctrl + S` to save a portable `.excalidraw` file as backup. |

---

## Release Notes — v1.0.0

First stable release.

- Single-file deployment (one HTML file, no dependencies)
- Full drawing toolset powered by Excalidraw
- Image shadow system with presets and custom controls
- Autosave to browser localStorage
- File operations: New, Open, Save, Export PNG
- Keyboard shortcuts for all tools
- Works offline, no server required
- Accessible: ARIA labels, keyboard navigation

---

## License

MIT
