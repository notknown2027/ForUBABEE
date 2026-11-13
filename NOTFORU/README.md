# A little website for Vruu

A responsive romantic memory book built with HTML, CSS and JavaScript. The final gift reveals the supplied ring photo.

## Run it

Because the project uses JavaScript modules, start a small local web server from this folder. For example, if Python is installed:

```powershell
python -m http.server 8000
```

Then open `http://localhost:8000`. The site password is `VRUSHAN2027`. This is a playful JavaScript privacy gate, not secure authentication: the password is visible in the client source and should not protect private information. The gift password is separate (`ILU27`) and only unlocks the gift scene.

## Add your photos and videos

The supplied files are also copied into `assets/images/` and `assets/videos/` using the names `photo-01.jpg` through `photo-17.jpg` and `video-01.mp4` through `video-04.mp4`. The supplied photos, videos, and music are included in the page. Use image files with the original framing; cards use `object-fit: cover`, and the lightbox shows the complete image. Use landscape or portrait dimensions suitable for web delivery and compress large files before adding them.

## Add instrumental music

The supplied music is copied to `assets/audio/alfaz-instrumental.mp3`. Playback starts only when the visitor taps the music control. If the file is missing, the control reports that audio is unavailable. The chosen play/pause state stays in place as visitors move between chapters.

## Deploy

Upload the project folder, preserving its structure, to any static hosting provider such as GitHub Pages, Netlify, or Cloudflare Pages. No build step is required. The display fonts are loaded from external CDNs and need an internet connection. For fully offline use, vendor those libraries and fonts locally.

## Project map

- `index.html` — opening password, 10 chapters, quiz, memory transition, and last-page gift.
- `css/` — base styles, animations, and responsive layouts.
- `js/main.js` — navigation, passwords, music, memories, gallery, lightbox, and quiz logic.
- `assets/images/`, `assets/videos/`, `assets/audio/` — add your own media here.

The chapter and gift passwords are client-side demonstrations; static hosting cannot hide credentials from someone inspecting downloaded source. Avoid putting sensitive content behind them.

The hamster starts beside the story; after a click it does a comic boop and darts to a safe random spot, then dodges a nearby cursor. The opening growth illustration is a custom animated rose garden SVG.
