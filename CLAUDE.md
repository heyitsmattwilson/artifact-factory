# Artifact Factory — CLAUDE.md

## What this is
A single-file HTML tool (`artifact_factory.html`) that generates client-ready sales and insights artifacts for Ibotta's **Insights 2.0** capability. Built by Matt Wilson (Client Analytics, Ibotta) with Claude.

The tool lives at:
- **Local**: `/Users/matt.wilson/artifact-factory/artifact_factory.html`
- **GitHub**: `https://github.com/heyitsmattwilson/artifact-factory`
- **Live (GitHub Pages)**: `https://heyitsmattwilson.github.io/artifact-factory/artifact_factory.html`

---

## What it does
A two-panel web UI:
- **Left panel (inputs)**: Client context fields (account, brand, category, contact, campaign period), client objective selector, audience segment selector
- **Right panel (outputs)**: Auto-generated artifacts that update in real time as inputs change

### Client Objectives
| Key | Label | Description |
|---|---|---|
| `profitable-growth` | Profitable Growth | Hit a CPID target, grow top + bottom line |
| `gap-close` | Gap Close | Hit a specific incremental sales volume |
| `new-hh` | New HH Penetration | Grow the buyer base with net-new shoppers |
| `market-share` | Market Share Defense | Recapture lapsed or competitive switchers |

### Audience Segments
| Key | Label |
|---|---|
| `loyal` | Loyal buyers |
| `lapsed` | Lapsed buyers |
| `new` | New households |
| `competitive` | Competitive switchers |

---

## Design
- **Single HTML file** — no build step, no dependencies, no server required
- **Ibotta brand colors**: orange (`#FF5A1F`), navy (`#1A2B4A`)
- Artifacts include SQL templates, narrative copy, and presentation-ready output blocks
- Outputs update live via `generate()` JavaScript function triggered on input changes

---

## How to share
- Open `artifact_factory.html` directly in any browser (local use)
- Share via GitHub Pages link above (no login required)
- Use `htmlpreview.github.io` as a fallback renderer for direct GitHub blob links

---

## Stack
- Pure HTML/CSS/JavaScript — no framework, no dependencies
- Deployed via GitHub Pages (auto-deploys on push to `main`)

---

## Owner
Matt Wilson — Client Analytics, Ibotta
`matt.wilson@ibotta.com`
