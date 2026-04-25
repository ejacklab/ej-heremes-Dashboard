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

## Planned

- [ ] MoneyFlow plugin tab — finance data inline
- [ ] Agent Hub tab — live status of all running agents (Lux, Apex, Sear, Orion)
