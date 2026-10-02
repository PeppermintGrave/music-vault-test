# Music Vault: Midnight Recordings

A cinematic, ambient web-based music player built as a single-page experience for a personal archive of recordings. This project turns a curated collection of atmospheric tracks into an immersive listening environment—complete with a dark, terminal-inspired interface, interactive visualizer, and a hand-built playlist experience.

## Overview

Music Vault is a lightweight static website that presents a collection of original or curated recordings as a "vault" of midnight transmissions. The experience is intentionally atmospheric: low-light UI, synth-like motion, fluorescent text, and a minimalist player layout inspired by retro terminal systems and modern ambient interfaces.

The project is intentionally simple and portable: it is a plain HTML, CSS, and JavaScript application with no framework or build step required. It is designed to run directly in a browser and can be served locally with a tiny static server.

## What this project does

- Loads a personal music library from local MP3 files
- Displays each track in an interactive playlist
- Supports play, pause, next, previous, shuffle, repeat, and seek controls
- Includes a dynamic visualizer and an ambient mode toggle
- Presents the experience in a moody, immersive aesthetic inspired by late-night archives and system consoles
- Runs entirely on the front end with embedded local audio assets

## Features

- Minimal static architecture: no dependencies or package installation required
- Responsive layout for desktop and mobile browsing
- Keyboard controls for quick playback interaction
- Custom visual equalizer bars and playback progress indicator
- Playlist metadata for each track
- Ambient visual mode for a more immersive presentation
- Local media assets stored directly in the repository

## Repository structure

```text
music-vault-test/
├── index.html
├── audios/
│   ├── Paper Moons.mp3
│   ├── Mosslight Drift.mp3
│   ├── Still Here.mp3
│   ├── When the Night Learns Your Name.mp3
│   ├── Old Notebook.mp3
│   ├── Static Skies.mp3
│   ├── Where the Silence Grows.mp3
│   ├── Where the Daylight Ends.mp3
│   ├── When You Still Knew Me.mp3
│   ├── From the Other Side of the Screen.mp3
│   └── ...
└── README.md
```

## Technical details

This repository is built with:

- HTML5 for structure
- CSS3 for styling and visual treatment
- Vanilla JavaScript for playback logic and interactivity
- MP3 audio files stored locally in the `audios` directory

The player is created from a `MUSIC_LIBRARY` array in `index.html`, where each track includes:

- the track title
- the associated file path
- metadata used for the player UI

The interface updates dynamically as the track changes, and the `audio` element handles playback and timing while the custom UI reflects state changes in real time.

## How to run

Because this is a static site, you can run it either by opening `index.html` directly in a browser or by serving it locally.

### Option 1: Open directly

Open `index.html` in your browser.

### Option 2: Run a local web server

From the repository root:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## Playback controls

The player includes:

- Play / Pause
- Previous / Next
- Shuffle
- Repeat
- Volume control
- Progress scrubbing
- Ambient mode toggle

Keyboard shortcuts are also supported:

- Space: play or pause
- Left Arrow: previous track
- Right Arrow: next track
- Up/Down Arrow: adjust volume

## Design philosophy

The visual language of the project is intentionally atmospheric and archival:

- dark green-black palette
- terminal-inspired panels
- minimal, elegant typography
- glowing accent colors for music cues
- motion and layering to simulate an active transmission or live archive

The overall identity evokes a private collection of emotional, nocturnal recordings preserved in a digital vault.

## Notes

- This project is built for personal or artistic use.
- The audio files are stored locally in the repository, making the project easy to distribute or archive.
- There is no backend, database, or external API dependency.

## License

This repository does not currently include a formal license file. Unless otherwise stated, all rights remain with the repository owner and original creator. If you intend to reuse or distribute the project, please confirm usage rights before doing so.

## Credits

Created and curated by PeppermintGrave.

## Summary

Music Vault: Midnight Recordings is a self-contained ambient music experience that packages a personal library into a richly styled, browser-based listening environment. It is simple, portable, and intentionally aesthetic—built to feel like a private archive of music preserved in a digital night-state.
