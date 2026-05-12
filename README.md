<div align="center">

<br/>

```
███████╗██╗  ██╗ ██████╗ ████████╗██╗     ██╗███████╗████████╗███████╗██████╗
██╔════╝██║  ██║██╔═══██╗╚══██╔══╝██║     ██║██╔════╝╚══██╔══╝██╔════╝██╔══██╗
███████╗███████║██║   ██║   ██║   ██║     ██║███████╗   ██║   █████╗  ██████╔╝
╚════██║██╔══██║██║   ██║   ██║   ██║     ██║╚════██║   ██║   ██╔══╝  ██╔══██╗
███████║██║  ██║╚██████╔╝   ██║   ███████╗██║███████║   ██║   ███████╗██║  ██║
╚══════╝╚═╝  ╚═╝ ╚═════╝    ╚═╝   ╚══════╝╚═╝╚══════╝   ╚═╝   ╚══════╝╚═╝  ╚═╝
```

**make shot lists the easy way.**  
kill all your subscritions please, were back to true indie filmmaking.

<br/>

[![Deploy to GitHub Pages](https://img.shields.io/badge/Deploy_to-GitHub_Pages-black?style=for-the-badge&logo=github)](https://pages.github.com/)
[![Made with HTML](https://img.shields.io/badge/Made_with-HTML%2FCSS%2FJS-f5d800?style=for-the-badge&logo=html5&logoColor=black)](https://github.com)
[![No frameworks](https://img.shields.io/badge/Zero-Dependencies-ff6b9d?style=for-the-badge)](https://github.com)
[![License MIT](https://img.shields.io/badge/License-MIT-3a6fff?style=for-the-badge)](LICENSE)

<br/>

</div>

---

## ▸ What is this?

**shotlister** is a single `index.html` file that turns any browser into a professional shot list tool — StudioBinder style, zero subscription. Drop it on GitHub Pages and share it with your whole crew. Everything saves locally in the browser. Nothing leaves the device.

Built for directors, ADs, DPs, and anyone who's ever tried to manage a shot list in a Google Sheet and wanted to cry.

---

## ▸ Features

### 🎬 Shot Management
- **Add, edit, delete** shots with a clean modal
- **Inline editing** — click any description, subject, location, or equipment cell and type
- **Double-click a row** to open the full edit modal
- **Bulk select + delete** via checkboxes
- **Upload a frame reference / storyboard image** per shot (stored locally)
- Shots **auto-sort** by scene → shot number

### 📋 Fields per Shot

| Category | Fields |
|---|---|
| **Core** | Scene #, Shot #, Description, Subject |
| **Camera** | Camera, Shot Size, Shot Type, Movement, Equipment, Frame Rate |
| **Production** | Sound, Location, Time of Shoot |
| **Lighting** | Setup, Time of Day, Colour Temp, Mood, Modifier, Notes |
| **VFX** | Type, Practical FX, Tracking, Complexity, Vendor, Notes |

### 📊 Stats Panel
Live dashboard showing:
- Total shots + scenes
- VFX shot count
- Framed shots (with image) + % complete progress bar
- Most-used camera movement

### 🔍 Filtering & Search
- Full-text search across all fields
- Filter by **scene number**
- Filter by **shot type**

### 💾 Export
- **Excel (.xlsx)** — full spreadsheet with all fields
- **CSV** — for any other tool
- **JSON** — raw data backup / restore
- **Print / PDF** — print-optimised layout

---

## ▸ Getting Started

### Option 1 — Just open it locally

```bash
# Download index.html, double-click it.
# Done.
```

No build step. No npm install. No webpack. Nothing.

### Option 2 — Just use the website buddy

```bash
# https://urmeankanha.github.io/shotlister/. enter.
# done.
```

seriously. just use the website


---

## ▸ Data & Storage

> **Your shots never leave your browser.**

shotlister uses `localStorage` — data is tied to the domain in your browser, not to the HTML file. This means:

- ✅ Updating the code **will not** delete saved shots
- ✅ Refreshing the page **will not** delete saved shots
- ❌ Clearing browser data / private mode **will** wipe shots
- ❌ Shots are **not synced** between devices or users

**Backup tip:** Use **Export → JSON** regularly to keep a copy of your data.

---

## ▸ Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `⌘ / Ctrl + N` | Add new shot |
| `Esc` | Close modal |
| `Double-click row` | Edit shot |

---

## ▸ Deploying Updates

When you push changes to `main`, GitHub Pages rebuilds automatically (usually within ~60 seconds). Users who refresh the page get the latest version. Their shot data is untouched.

```
Push to main → GitHub Pages rebuilds → users refresh → data still there ✓
```

---

## ▸ Customising

Everything is in one file — open `index.html` in any editor.

**Change the colour palette** → edit the `:root` CSS variables at the top:

```css
:root {
  --yellow: #f5d800;   /* primary accent */
  --pink:   #ff6b9d;   /* secondary accent */
  --blue:   #3a6fff;   /* links / pills */
  --ink:    #111111;   /* text + borders */
  --bg:     #f7f3ec;   /* page background */
}
```

**Add a new field** → add an input to the modal HTML, include the field name in `ALL_FIELDS`, and add a column header + cell to `mkRow()`.

---

## ▸ Tech Stack

```
HTML5          — structure
CSS3           — layout, animations, neo-brutalist design system
Vanilla JS     — all logic, no frameworks
localStorage   — persistence
SheetJS        — .xlsx export (loaded from CDN)
Syne + Inter   — typography (Google Fonts)
```

---

## ▸ License

MIT — do whatever you want with it. Credit appreciated but not required.

---

<div align="center">

**Made for filmmakers. Free forever.**

[![Open in Browser](https://img.shields.io/badge/▶_Open_in_Browser-black?style=for-the-badge)](https://yourusername.github.io/shotlister)
[![Report a Bug](https://img.shields.io/badge/🐛_Report_a_Bug-ff3636?style=for-the-badge)](https://github.com/yourusername/shotlister/issues)
[![Request a Feature](https://img.shields.io/badge/✦_Request_Feature-f5d800?style=for-the-badge&logoColor=black)](https://github.com/yourusername/shotlister/issues)

<br/>

*go make something.*

</div>
