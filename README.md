# macOS Portfolio

A personal portfolio website themed after macOS — mimicking a Mac desktop with a menu bar, wallpaper, dock, and windowed applications.

Built with **React 19**, **Vite 8**, **Tailwind CSS v4**, and **GSAP** for animations.

## Tech Stack

| Category | Technologies |
|---|---|
| Framework | React 19 |
| Build Tool | Vite 8 |
| Styling | Tailwind CSS v4, Google Fonts (Georama, Roboto Mono) |
| Animation | GSAP 3 + `@gsap/react` |
| Linting | oxlint (Rust-based) |
| Icons | Custom SVGs + Lucide React |

## Getting Started

```bash
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

## Scripts

| Script | Command |
|---|---|
| `dev` | `vite` — start dev server |
| `build` | `vite build` — production build |
| `preview` | `vite preview` — preview production build |
| `lint` | `oxlint` — run linter |

## Project Structure

```
src/
├── main.jsx              # Entry point
├── App.jsx               # Root component
├── index.css             # Global styles + Tailwind + component CSS
├── components/
│   ├── index.js          # Barrel exports
│   ├── Navbar.jsx        # macOS-style top menu bar
│   └── Welcome.jsx       # Hero section with GSAP text animation
└── constants/
    └── index.js          # Portfolio data (nav, dock, projects, blog, etc.)
```

## Features

- **macOS desktop metaphor** — wallpaper, menu bar, app dock, and draggable windows
- **Interactive hero** — GSAP-powered font-weight morphing that responds to cursor movement
- **Window management infrastructure** — z-index layering and window config ready for Finder, Safari, Terminal, Photos, Contact, and Resume "apps"
- **Dark/Light mode** — toggle support via the navbar

## Author

**Aryan Khaund** — aryan.khaund@gmail.com
