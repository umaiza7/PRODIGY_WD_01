# AFTERGLOW

**Music for the hours when the day is over but your mind isn't.**

A single-page mixtape landing site for *AFTERGLOW*, a fictional late-night alternative R&B / indie playlist. Built as a one-file HTML/CSS/JS design piece — no frameworks, no build step.

**Live site:** https://umaiza7.github.io/PRODIGY_WD_01/

## About

AFTERGLOW leans into a mixtape-spread concept rather than a typical product page: an oversized wordmark hero with ambient glow and film grain, a tilted "cover art" spread built entirely from CSS/SVG, and a two-column **Side A / Side B** tracklist that tells a small story through time-stamped labels — *11:47 PM · getting home* and *2:13 AM · not going to sleep*.

All copy — track titles, artist names, the tagline — is realistic placeholder content for a fictional brand. All artwork (ripple/sphere cover, grain vignette, cassette-style motifs) is original CSS/SVG, not sourced imagery.

## Features

- Fixed, sticky nav with smooth-scroll anchor links
- Oversized gradient wordmark hero with layered ambient glow and a film-grain overlay
- Two abstract cover-art cards built with pure CSS gradients and SVG — no image assets
- Side A / Side B tracklist styled as liner notes, with hover states per track
- Fully responsive down to mobile
- Zero dependencies — one `index.html` file, inline CSS and JS

## Tech

Plain HTML, CSS, and vanilla JavaScript. No build tools, no package manager, no external fonts or libraries — everything (including the grain texture) is generated inline via CSS/SVG so the page loads as a single static file.

## Running locally

```bash
git clone https://github.com/umaiza7/PRODIGY_WD_01.git
cd PRODIGY_WD_01
open index.html
```

Or serve it with any static server, e.g. `python3 -m http.server`.

## Customizing

- **Streaming link:** every "Listen Now" button shares a `data-listen-link` attribute — swap the placeholder `href="#"` on those four buttons for a real Spotify / Apple Music / YouTube playlist URL.
- **Colors:** the palette lives as CSS custom properties at the top of the stylesheet (`--ink`, `--rust`, `--dust`, `--glow`, etc.).
- **Tracklist:** edit the `.track` rows inside the `#tracks` section directly in `index.html`.

## Deployment

Hosted with GitHub Pages, serving straight from the `main` branch root.
