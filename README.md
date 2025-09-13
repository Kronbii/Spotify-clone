# Spotify Clone (Static UI)

A responsive front-end clone of Spotify's desktop application interface built with vanilla HTML and CSS. This project focuses on layout, styling, and component structure (no JavaScript logic or backend yet). It recreates the sidebar navigation, library section, playlist view, and footer playback controls for a realistic UI demo.

## 🎯 Goals
- Practice semantic structuring and modular CSS
- Recreate a complex modern music app layout
- Establish a clean foundation for later interactivity (player controls, dynamic playlists, etc.)

## ✨ Features (Current)
- Left sidebar: Home, Search, Your Library filters
- Library list with pinned / playlist metadata
- Playlist view with header (artwork, metadata, actions)
- Scrollable track list with columns (Title, Album, Date Added, Duration)
- Footer player bar with transport controls and progress/volume sliders
- Custom fonts via Google Fonts (Montserrat & Nunito)
- SVG icon set + cover images stored locally
- Accessibility improvements (alt attributes + ARIA labels)

## 🧱 Tech Stack
- HTML5 (static markup)
- CSS3 (multiple modular stylesheets)
- Local assets (SVGs + JPEG/PNG)

_No build system required — open the HTML file directly._

## 📂 Project Structure
```
root/
  index.html              # Main entry (previously src/spotify.html)
  README.md
  LICENSE
  .gitignore
  font/                   # Local font assets (if needed later)
  iconss/                 # (Legacy bulk SVG set – audit & prune)
  src/
    icons/                # Icons actually referenced in UI
    song-images/          # Playlist / track artwork & profile images
    styles/
      base/               # Global tokens, variables, resets
      layout/             # Structural layout (containers, grids)
      components/         # Reusable UI pieces (header, footer)
      pages/              # Page-level styling (playlist, library, home)
```

### Unused / To Review
The top-level `iconss/` directory contains many numbered SVGs not referenced in `index.html`. Consider pruning or moving only required assets into `src/icons/`.

## 🚀 Getting Started
1. Clone the repository:
```bash
git clone https://github.com/<your-username>/Spotify-clone.git
cd Spotify-clone
```
2. Open `index.html` in a browser:
```bash
xdg-open index.html   # Linux
open index.html       # macOS
start index.html      # Windows (cmd)
```
3. (Optional) Serve with a lightweight dev server for future JS work:
```bash
python3 -m http.server 5173
# then visit http://localhost:5173
```

## 📌 Roadmap Ideas
| Phase | Upgrade |
|-------|---------|
| 1 | Add JavaScript for play/pause button state toggle |
| 2 | Extract repeated components (playlist item) into templates |
| 3 | Introduce a JSON data file for dynamic track rendering |
| 4 | Implement a lightweight audio player (HTML5 `<audio>` tag) |
| 5 | Theme switching (light/dark/contrast) |
| 6 | Responsiveness improvements & mobile layout |
| 7 | Deploy via GitHub Pages or Netlify |
| 8 | Asset pruning & performance pass (image optimization) |

## 🧹 Future Enhancements / Refactor Opportunities
- Consolidate repetitive spacing & colors into CSS variables
- Create a utility layer (e.g., spacing helpers, flex helpers)
- Consider a preprocessor (Sass) only if complexity grows
- Replace hard-coded widths with responsive flex/grid patterns
- Add Lighthouse + accessibility audit script

## 🛡️ License
MIT © 2025 Your Name

## 🤝 Contributing
Feel free to fork and submit PRs. For larger changes, open an issue first to discuss structure or direction.

### Preferred Style
- Use semantic class naming (BEM-ish or clear functional names)
- Keep component-specific styles scoped to their CSS file
- Avoid inline styles to preserve separation of concerns

## 📷 Screenshots (Optional)
Add screenshots here (e.g., `docs/screenshots/playlist-view.png`).

## 💡 Tips for Next Steps
- Minify or consolidate CSS once structure stabilizes
- Add a favicon and meta tags for better presentation
- Use `:root` CSS variables for color palette + spacing scale
- Extend alt text for more context (currently concise)

---
Happy to help implement any of the roadmap items—just ask!
