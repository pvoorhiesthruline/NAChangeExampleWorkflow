# ADKAR × COM-B Overlay

A single-file HTML reference document overlaying Prosci's ADKAR model with Michie, van Stralen & West's COM-B system (Behaviour Change Wheel, 2011), plus a deliverable map of typical change management templates by phase (Inputs, Change Discovery, Change Strategy, Change Implementation).

## Structure

Everything lives in `index.html`:
- Inline `<style>` block at the top (design tokens as CSS custom properties under `.acw-root`, prefixed `acw-`)
- Markup below is organized into two sections: the ADKAR/COM-B matrix (`01 — The overlay`) and the deliverable map (`02 — Deliverable map`)
- No build step, no dependencies beyond the Google Fonts import (Fraunces, Inter, IBM Plex Mono) — open `index.html` directly in a browser

## Editing notes

- Deliverable cards use `.acw-card`, with `.acw-tag-row` for ADKAR/COM-B tags and `.acw-links` for template links
- Phase groupings use `.acw-phase` / `.acw-phase-head`
- Colors: `--cap` (capability, green), `--opp` (opportunity, blue), `--mot` (motivation, ochre) — reused across matrix cells, tag pills, and section accents
