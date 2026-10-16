# Presentations — Hélder Palheira

AI, Digital Health and Health Informatics presentations by Hélder Palheira. Slide decks
covering Generative AI, Clinical Informatics, Digital Transformation, Nursing Informatics,
Interoperability, Evidence-Based Healthcare, and Innovation in Health Systems.

Built with [reveal.js](https://revealjs.com/). Each deck is a **single, self-contained
HTML file** — all CSS and animations inlined directly in the file (no separate stylesheet
to track). This makes every deck trivial to download and share through any channel (email,
Slack, USB) and open directly in a browser, with no build step. Reveal.js and Font Awesome
still load from CDN, so an internet connection is needed to render — only the styling and
structure are self-contained.

🔗 **Live decks:** https://hasp7.github.io/presentations/

## Structure

Decks are grouped by domain, one folder per topic area:

```
/
├── index.html                       ← landing page, links to all decks
├── genai/
├── clinical-informatics/
├── digital-transformation/
├── nursing-informatics/
├── interoperability/
├── evidence-based-healthcare/
├── innovation-in-health-systems/
└── clients/                       ← propostas a clientes; não listadas no index, com noindex
```

Each folder holds one `.html` file per deck (`<deck-slug>.html`), fully self-contained.

## Workflow: publishing a deck from the HQ

Decks are drafted in a private workspace (Claude Code + the `/revealjs` skill), then
published here once ready to share:

1. Build the deck as usual (produces `presentation.html` + `styles.css`).
2. Inline `styles.css` into a single `<style>` block in the HTML `<head>`, and remove the
   external stylesheet `<link>` — the file must stand on its own.
3. Rename to a descriptive slug and place it under the matching domain folder
   (`<domain>/<deck-slug>.html`).
4. Add a link to it from the root `index.html`.
5. Commit and push — GitHub Pages picks it up automatically.

## License

Content © Hélder Palheira. Slides are shared for reference; reuse requires attribution.
