# Gratitude – Daily Reflections

A minimal, browser-based gratitude journal that helps you capture daily moments of appreciation. Each entry is paired with unique generative artwork, creating a personal and visually rich record of gratitude over time.

## Features

- **Daily journaling** — Write one gratitude entry per day (up to 500 characters) with a clean, distraction-free interface.
- **Generative artwork** — Each entry gets a unique, deterministic piece of canvas-based art derived from the content you write.
- **Journal view** — Browse all past entries in a responsive grid with relative dates ("Today", "Yesterday", "3 days ago").
- **Export / Import** — Back up your journal as a JSON file and restore it later. Imports merge with existing data without overwriting.
- **Privacy-first** — All data is stored in the browser's `localStorage`. Nothing is sent to a server.

## Tech Stack

- **HTML / CSS / JavaScript** — Single-file application (`index.html`), no build step or framework required.
- **Canvas API** — Procedurally generated artwork using gradient blobs, geometric shapes, and noise textures.
- **Google Fonts** — DM Serif Display (headings) and Inter (body text).
- **localStorage** — Persistent client-side storage under the key `golden_hour_entries`.

## Getting Started

Open `index.html` in any modern browser. No server, bundler, or installation is needed.

```sh
# or serve locally
npx serve .
```

## Data Format

Entries are stored as a JSON array:

```json
[
  {
    "date": "2026-02-04",
    "text": "Grateful for a quiet morning walk.",
    "time": "8:15 AM"
  }
]
```

## Design

The interface uses a warm palette — terracotta, teal, sand, and cream — with smooth transitions and a mobile-first responsive layout that switches from a two-column grid to a single column below 640px.
