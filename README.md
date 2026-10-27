# Cryptography End-Sem Prep · MJPRU CS-443T

Study site for **MJPRU Bareilly · B.Tech VII Semester · Network Security and Cryptography (CS-443T)**.

**[Open the site](https://hira04irshad.github.io/crypto-mjpru-prep/)**

## What's inside

| Page | What it gives you |
|---|---|
| **PYQ analysis** | The 2025-26 end-sem and both 2025 mid papers ranked by topic, the numericals, and a predicted paper |
| **All past papers** | Every question typed out and tagged by unit, with the answer to every numerical, plus the syllabus |
| **How to write answers** | The MJPRU long-answer template, protocol diagrams, and the layout for numericals |
| **Video lectures** | YouTube lectures for every syllabus topic, unit by unit; tap to play on the page |
| **Unit notes 1–5** | The full syllabus (Schneier), with every PYQ numerical solved step by step: Playfair, Hill, columnar, Diffie–Hellman, RSA, Shamir, blind signatures, Fiat–Shamir |
| **Mock papers 1–3** | 70-mark papers in the MJPRU pattern (any 5 of 8) with full answers; every numerical checked by computer |
| **Last-night sheet** | Definitions, lists, formulas, the numerical answers, diagrams to practise |

## How it works

A static site with no build step, using the same design as [dip-mjpru-prep](https://github.com/arshanalikhan/dip-mjpru-prep) and [cyber-mjpru-prep](https://github.com/HIRA04IRSHAD/cyber-mjpru-prep): sidebar on desktop, top bar and bottom tabs on phones, light and dark themes. `index.html` holds the shell and the home page; every other page is `content/<page>.md`, loaded for the page in the URL hash and rendered with [marked](https://marked.js.org/). ` ```mermaid ` blocks are drawn with [Mermaid](https://mermaid.js.org/), `::: ans` / `::: tip` / `::: warn` blocks become styled boxes, and `@yt id | title | channel | length` lines become video cards. Progress ("mark as done") and exam mode are saved in the browser only.

```text
index.html          shell (sidebar, phone tabs) and the home page
assets/base.css     design tokens, shell and home styles
assets/cr.css       additions: Markdown pages, diagrams, answer boxes, topic bars, video cards
assets/app.js       router, Markdown + diagrams + videos, progress, exam mode, hero animation
content/*.md        every other page
```

To edit content, change the Markdown in `content/` and push to `main`; GitHub Actions publishes to GitHub Pages. When you change `assets/`, bump the `?v=` number in `index.html`. The end-sem date is `EXAM_DATE` in `assets/app.js` (a tentative 15 Dec 2026).

Preview locally:

```bash
python -m http.server 8795
```

## Sources

The syllabus follows Bruce Schneier, *Applied Cryptography* (chapters 1–5, 8, 10), with Stallings, *Cryptography and Network Security*, for MACs, public-key distribution, DES and AES. The papers are from our batch (2025-26); no older MJPRU CS-443T papers could be found online.

Not an official MJPRU resource. If anything here disagrees with your class notes, trust your teacher.
