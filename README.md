# jacksonkustin.com

Personal site — AI systems builder portfolio. Static HTML/CSS/JS, no build step, hosted on GitHub Pages.

## Structure

```
index.html                    Home (hero → trust → manifesto → work → process →
                              capabilities → bio → fit → testimonials → FAQ → CTA)
work.html                     All projects
about.html                    Long-form bio
resume.html                   Inline PDF + download
book-a-call.html              Intake form + scheduler slot
project-*.html                Individual case studies
assets/css/site.css           All styling. Design tokens are the :root vars at the top.
assets/js/site.js             Mobile nav, sticky header, scroll reveal
assets/img/                   Photos + screenshots (drop files here)
```

## Design tokens

Everything is driven by CSS custom properties in `assets/css/site.css`:

| Token | Value | Use |
|---|---|---|
| `--cream` | `#F4F1EA` | Page background |
| `--sand` | `#EAE4D6` | Alternating section background |
| `--tan` | `#DDD2B4` | Image placeholder fill |
| `--ink` | `#15140F` | Text, dark sections, primary buttons |
| `--orange` | `#E8501F` | Accent, eyebrows, links, hover state |

Type: Space Grotesk (display) · Instrument Serif (italic accents) · IBM Plex Sans (body) · IBM Plex Mono (labels).

## Local preview

```bash
python3 -m http.server 4321
```

Then open http://localhost:4321.

## TODO before launch

- [ ] Replace the two `PHOTO PLACEHOLDER` blocks (home hero + about) with real photos
- [ ] Replace `SCREENSHOT PLACEHOLDER` / `APP SCREEN PLACEHOLDER` blocks with real product shots
- [ ] Write real testimonials, or delete the testimonials `<section>` in `index.html`
- [ ] Fill the two `[PLACEHOLDER]` FAQ answers (pricing, timeline)
- [ ] Fill in project case study copy (Problem / stage descriptions)
- [ ] Set the Formspree endpoint in `book-a-call.html` (`action="..."`)
- [ ] Paste the Calendly embed in `book-a-call.html` (marked with a comment)
- [ ] Add `CNAME` if using a custom domain
