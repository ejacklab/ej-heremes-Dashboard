# Hermes Dashboard Themes

Custom themes for the Hermes Agent dashboard. All themes are designed with accessibility-first principles: high contrast, colorblind-safe, and elder-friendly.

## Themes

| # | Name | Accent | Description |
|---|------|--------|-------------|
| 001 | Nightwave | Cyan + Orange | Near-black navy with steel-blue chrome and icy cyan |
| 002 | Oxide | Chartreuse | Acidic chartreuse on warm-black with amber bokeh |
| 003 | Voltis | Cyan + Gold | Deep teal command center with electric cyan chrome |
| 004 | Helios | Amber + Blue | Deep navy command center — amber-gold accent, colorblind-safe |
| 005 | Aether | Cyan + Amber | Dark cyan command center — high contrast, elder-friendly |
| 006 | Luminos | Gold + Teal | Warm amber-gold retro-futuristic command center |
| 007 | Cipher | Blue + Gold | Cool blue holographic command center |
| 008 | Aureus | Gold + Teal | Warm golden cosmic command center |
| 009 | Opus | Gold + Orange | Luxurious golden fintech command center |
| 010 | Verdant | Lime + Orange | Vibrant lime-green neon command center |
| 011 | Nexus | Blue + Amber | Cool blue cyberpunk command center |
| 012 | Aurora | Cyan + Gold | Electric cyan aurora command center |
| — | Bastion | Terracotta | Military ops olive-green with terracotta accent |
| — | Garrison | Terracotta + Blue | Bright olive command center — high-contrast, section-colored |
| — | Lux | Cyan | Deep indigo command center with electric cyan accent |

## Accessibility Standards

All themes comply with:

- **WCAG 2.2 AA** minimum (4.5:1 contrast for text)
- **WCAG AAA** target (7:1) for primary text and KPIs
- **Colorblind-safe**: No red/green semantic pairing. Success = blue-teal, Destructive = orange-red
- **Elder-friendly**: 15px base font, 1.6 line height, 0.02em letter spacing, comfortable density
- **Focus rings**: 2px thick (WCAG 2.4.11)
- **Chart strokes**: 2.5px minimum
- **Scrollbar**: 6px width for grab targets

## Installation

Copy the YAML files to your Hermes dashboard themes directory:

```bash
cp *.yaml ~/.hermes/dashboard-themes/
```

For themes with background images (006–012), copy the bg-assets to the
web public directory so the dashboard can serve them:

```bash
cp bg-assets/*.png ~/.hermes/hermes-agent/web/public/ds-assets/
cp bg-assets/*.jpg ~/.hermes/hermes-agent/web/public/ds-assets/
```

Then rebuild the frontend and restart the dashboard:

```bash
cd ~/.hermes/hermes-agent/web && npm run build
hermes dashboard --no-open
```

Select the theme from the picker at http://127.0.0.1:9119.

## Background Images

Themes 006–012 use custom background images (`assets.bg`). These render at ~4.5% opacity with `difference` blend mode — subtle texture, not overpowering.

## File Structure

```
.
├── *.yaml                    # Theme definitions
├── bg-assets/                # Background images for themes
│   ├── 006bg.png – 012bg.png
│   └── filler-bg0.jpg        # Default dashboard filler
├── reference-images/         # Source reference images
│   └── 001.png – 012.png
└── README.md
```
