# Mudit Chopra — AI Creative Producer

Editorial portfolio website. Concept-driven spec films, commissioned brand
work, and AI content systems.

## Stack
Static site — a single `index.html` (no build step) with a hash-based router
for case-study pages. Assets live in `assets/`.

```
index.html
assets/
  logos/   13 brand logos
  video/   5 optimized MP4s + posters + selected frames
```

## Content
- **Lead Stories** — two independent spec films (FirstClub, Sleepy Owl), each
  with a full case-study page (concept → method → selected frames → final film).
- **Good Company** — grid of 13 brands experienced through agency roles.
- **Films in Motion** — commissioned brand films (Amazon Smart Commerce, ITC
  Aashirvaad, Notyetbyus) playing inline, plus published reels.
- **The Creative Desk / Systems / Byline** — content work, AI agents, contact.

## Videos
Source masters were re-encoded for web with ffmpeg (H.264, `+faststart`):
the two spec films were downscaled 1440×2560 → 1080×1920; the already-efficient
commissioned films were losslessly remuxed. Total media ≈ 48 MB (from 147 MB).

## Deploy
Static deploy on Vercel (no framework). Push to `master` to trigger a
production deployment. Previous version preserved on branch
`backup/portfolio-deck`.
