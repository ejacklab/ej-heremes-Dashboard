# Hermes Dashboard Themes

Custom themes for the Hermes Agent dashboard.

## Themes

| # | Name | Accent | Description |
|---|------|--------|-------------|
| 001 | Oxide | Chartreuse | Acidic chartreuse on warm-black with amber bokeh |
| 002 | Helios | Amber + Blue | Navy command center — amber-gold accent, colorblind-safe |
| 003 | Aureus | Gold + Teal | Warm golden cosmic command center |
| 004 | Opus | Gold + Orange | Luxurious golden fintech command center |
| 005 | Garrison | Terracotta + Blue | Bright olive command center — high-contrast, section-colored |

## Installation

```bash
# 1. Copy theme files
cp *.yaml ~/.hermes/dashboard-themes/

# 2. Copy background images
cp bg-assets/*.png ~/.hermes/hermes-agent/web/public/ds-assets/

# 3. Rebuild and restart
cd ~/.hermes/hermes-agent/web && npm run build
hermes dashboard --no-open
```

Select a theme from the picker at http://127.0.0.1:9119.

## File Structure

```
.
├── *.yaml                 # Theme definitions (001–005)
├── bg-assets/             # Background images
│   └── 001bg.png – 005bg.png
├── reference-images/      # Source reference images
└── README.md
```
