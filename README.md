# ej-hermes-Dashboard

Custom themes and plugins for the [Hermes Agent](https://hermes-agent.nousresearch.com) web dashboard.

## Themes

### Lux (`lux.yaml`)

Deep indigo command center. Electric cyan accent, sharp geometry, JetBrains Mono data readouts.

**Install:**
```bash
cp lux.yaml ~/.hermes/dashboard-themes/lux.yaml
```

Then open the dashboard, click the palette icon in the header, and select **Lux**.

**What it changes:**
- Palette: void-black `#080b18` base → cool periwinkle text → electric cyan `#00e5ff` accents
- Typography: Space Grotesk (body) + JetBrains Mono (code/data), 14px compact scale
- Layout: 0.25rem radius (sharp micro-bevel), compact density
- Components: gradient cards with cyan inset border, angled tabs, slim cyan scrollbars
- Chart bars: cyan gradient replacing the default washed-out beige
- Cost values: mint green `#00ffa3` for positive financial data
- Subtle scanline texture overlay

### Bastion (`bastion.yaml`)

Military ops / topographic aesthetic. Olive forest greens, warm cream text, terracotta accent — straight from the palette `#040302 → #181D11 → #2C3621 → #4F5A42 → #839177 → #9FAE97 → #C5BE94 → #DFDCC3` with `#B26948` terracotta for trend lines, CTAs, and live badges.

**Install:**
```bash
cp bastion.yaml ~/.hermes/dashboard-themes/bastion.yaml
```

Then open the dashboard → palette icon → **Bastion**.

**What it changes:**
- Palette: void black → olive panel layers → warm cream text → terracotta accent
- Typography: DM Sans (body) + IBM Plex Mono (data readouts)
- Cards: gradient from `#2C3621` → `#181D11` with olive inset border
- Topo texture: scanlines + crosshatch grid overlay (screen blend)
- Nav active: terracotta left bar + background tint
- Chart trend lines: terracotta `#B26948`
- Stat numbers: `#DFDCC3` warm cream highlight
- Card titles: uppercase small-caps `#DFDCC3`
- Slim 4px olive scrollbars
- Live badges: terracotta glow pulse

---

## Planned

- [ ] MoneyFlow plugin tab — finance data inline
- [ ] Agent Hub tab — live status of all running agents (Lux, Apex, Sear, Orion)
