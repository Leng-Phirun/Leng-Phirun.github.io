# Icons

## Inventory

**Brand logos** (from the contact section of the source site — inlined SVGs, extracted verbatim):
- `github.svg` — GitHub octocat, 24×24, filled, uses `currentColor`.
- `hackthebox.svg` — HTB hex logo, 24×24, filled.
- `tryhackme.svg` — THM shield mark, 24×24, filled.

**UI glyphs** (hand-rolled in the source with `stroke="currentColor"`, stroke-width 2):
- `ui/sun.svg` — theme toggle light state.
- `ui/moon.svg` — theme toggle dark state.
- `ui/arrow-up.svg` — back-to-top FAB.

All icons use `currentColor` — paint them by setting `color` on the parent.

## Usage

```html
<!-- Inline (recommended) -->
<a href="#" style="color: var(--accent)">
  <svg width="18" height="18"><use href="assets/icons/github.svg#root"/></svg>
</a>

<!-- Or via <img> (no recoloring) -->
<img src="assets/icons/github.svg" width="18" height="18" alt="GitHub">
```

## Emoji substitutes (pending approval)

The source uses **emoji via HTML entities** for certification and CTF category icons. These render inconsistently across OSes and weaken the hacker aesthetic. Proposed Lucide substitutions:

| Emoji | Entity | Used for | Proposed Lucide |
|---|---|---|---|
| 🛡 | `&#x1f6e1;` | OSCP | `shield` |
| 🎯 | `&#x1f3af;` | CRTA | `target` |
| 🔍 | `&#x1f50d;` | CREST CRT/CPSA | `search` |
| 💻 | `&#x1f4bb;` | PT1 | `laptop` |
| 🌐 | `&#x1f310;` | API Pentesting | `globe` |
| 🔒 | `&#x1f512;` | ISC2 CC | `lock` |
| 🎓 | `&#x1f393;` | Degree | `graduation-cap` |
| 📦 | `&#x1f4e6;` | HackTheBox card | `box` |
| 🚩 | `&#x1f6a9;` | TryHackMe card | `flag` |
| 🏆 | `&#x1f3c6;` | CTF Competitions | `trophy` |

**CDN:** `https://unpkg.com/lucide-static@latest/icons/{name}.svg`

Lucide is MIT-licensed, stroke-based, and visually aligns with the existing `sun.svg` / `moon.svg` / `arrow-up.svg` UI glyphs.

**Action required:** confirm whether to migrate to Lucide or keep emoji.
