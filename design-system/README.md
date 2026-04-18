# Phirun Cybersec — Design System

A terminal-native design language extracted from [Leng-Phirun.github.io](https://leng-phirun.github.io). Phosphor-green on near-black, CRT scanlines, katakana rain, glitch typography.

**Live:** <https://leng-phirun.github.io/design-system/>

## What's here

```
design-system/
├── index.html          # browsable viewer — open this first
├── tokens.css          # all design tokens (drop-in CSS variables)
├── ui-kit.html         # full portfolio page with Tweaks panel
├── assets/
│   └── icons/          # brand + UI + Lucide SVGs
└── previews/           # 23 component spec cards
```

## Using the tokens

Link `tokens.css` and use variables anywhere:

```html
<link rel="stylesheet" href="/design-system/tokens.css">
```

```css
.my-button {
  background: var(--accent);
  color: var(--bg-primary);
  font-family: var(--font-mono);
  padding: var(--sp-3) var(--sp-5);
  border-radius: var(--r-md);
  box-shadow: var(--shadow-btn-glow);
}
```

## Themes

| Attribute                | Effect                                 |
|--------------------------|----------------------------------------|
| `data-theme="dark"`      | default — phosphor on near-black       |
| `data-theme="light"`     | inverted — forest green on paper       |
| `data-accent="dim"`      | softer `#00cc6a` — easier on the eyes  |

Combine: `<html data-theme="dark" data-accent="dim">`

## The Tweaks panel

`ui-kit.html` exposes a bottom-right panel to flip accent · matrix density · CRT effects live. Great for screen-sharing and picking the exact vibe.

## Credits

- Brand SVGs: GitHub, HackTheBox, TryHackMe (trademarks of their owners)
- Category icons: [Lucide](https://lucide.dev) — ISC license
- Fonts: Inter + JetBrains Mono via Google Fonts

---

`> stay sharp_`
