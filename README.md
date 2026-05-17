# Spotify Clone 🎵

A responsive, high-fidelity Spotify web player replica built entirely from scratch using native vanilla web technologies. The application interfaces with a structured local storage directory to dynamically render albums, parse track listings, and control seamless audio streaming.

🔗 **Live Demo:** [View Live Deployment on Vercel](https://spotify-clone-wheat-seven.vercel.app/)

---

## 🚀 Key Technical Features

* **Dynamic Folder Parsing Async/Await:** Leverages client-side asynchronous JavaScript `fetch()` requests to navigate directories, automatically retrieving track data and reading album metadata JSON structures (`info.json`) on runtime initialization.
* **Liquid Breakpoints & Mobile Responsiveness:** Custom media queries (`@media (max-width: 1200px)`) built from scratch to transition from a full-width desktop 3-pane dashboard down to a compact mobile deck layout with slide-out sidebar navigation overlays.
* **Robust Custom Media Pipeline:** Powered by the HTML5 Audio API. Integrates custom timeline scrubbing via seekbar progression calculations, dynamic volume range input fields, and track jumping sync logic (Next/Previous navigation trackers).
* **Modular Clean Styling:** Utilizes dedicated layout partitioning with a core `style.css` for grid structures and a `utility.css` file managing design properties (flex distributions, text truncation, and customized webkit scrollbars).

---

## 📂 Repository Workspace Architecture

```text
├── .vscode/          # Local editor workspace configurations
├── img/              # Application UI graphics and asset vectors
├── songs/            # Track storage organized by explicit album folders
│   └── [Album-Name]/
│       ├── info.json # Metadata file containing playlist card text descriptors
│       └── cover.jpg # Target playlist card background graphic
├── favicon.ico       # Browser tab asset
├── index.html        # Main app view framework (Sidebar deck, Playlists grid, Media bar)
├── script.js         # Core logic: asynchronous directory scraping, track audio loops
├── style.css         # Visual aesthetic properties, grid spacing engines, media layouts
└── utility.css       # Layout helper classes, scrollbar styling, clean flex behaviors
