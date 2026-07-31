# jubinshaikh.github.io

Personal portfolio site for **Jubin Shaikh**  Computer Science, University of
Cincinnati. Full-stack and applied AI work, with every listed project deployed
and clickable.

**Live:** https://jubinshaikh.github.io/

## About

A hand-built static site  no framework, no build step, no dependencies beyond
webfonts. The whole thing is three files and a folder of images, which keeps it
fast and means there is nothing to break on deploy.

Sections: intro, selected work, stack, experience, contact.

## Stack

| Layer | Choice |
| --- | --- |
| Markup | Semantic HTML5 |
| Styling | Hand-written CSS with custom properties, no framework |
| Behavior | Vanilla JavaScript scroll reveals, nav state |
| Type | Source Serif 4, Inter, JetBrains Mono |
| Hosting | GitHub Pages |
| Analytics | Cloudflare Web Analytics (cookieless) |

## Structure

```
index.html          Main portfolio page
waph.html           Course project page (WAPH, archived)
css/style.css       All styling
js/script.js        All behavior
assets/img/         Profile image, screenshots, favicon
WAPH.md             Original course submission writeup
```

## Selected work

Each project on the site follows a Problem / Build / Outcome format and links to
both a live deployment and its source.

| Project | Focus |
| --- | --- |
| L'Oréal Routine Builder | Product-grounded LLM routine generation, RTL, persistence |
| L'Oréal Beauty Advisor | Domain-scoped chat with conversation memory |
| NASA Space Explorer | Public API integration with debounce and error states |
| Kanban Task Board | Drag-and-drop with localStorage persistence |
| Hydration Heroes | Browser game with a score/lives state machine |
| Intel: Sustainability Through the Ages | Interactive timeline, progressive disclosure |
| Sustainability Summit Check-In | Vanilla-JS state machine, capacity logic |

Both L'Oréal apps route API calls through a Cloudflare Worker so no API key is
ever exposed to the browser.

## Run locally

No build step. Clone and open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Analytics

Cloudflare Web Analytics is enabled via a beacon snippet in `index.html` and
`waph.html`. It is cookieless and collects no personally identifying
information, so the site needs no consent banner. Numbers should be read as a
floor rather than exact  ad blockers prevent the beacon from loading for some
visitors.

## Deploying

GitHub Pages builds from `main` automatically. Push and wait about a minute.
Pages caches aggressively, so hard refresh with `Ctrl+Shift+R` to confirm a
change actually landed.

## Course archive

This repository began as coursework for **Web Application Programming and
Hacking (WAPH)** with Dr. Phu Phung. The original submission writeup, covering
the Bootstrap build, jQuery clocks, cookie-based returning-visitor detection,
and public API integrations, is preserved in [`WAPH.md`](WAPH.md). The project
PDFs and `waph.html` remain in the repository for reference. The current site is
a full rewrite and shares no code with that version.

## Contact

- Email — shaikhjn@mail.uc.edu
- GitHub — [@Jubinshaikh](https://github.com/Jubinshaikh)
