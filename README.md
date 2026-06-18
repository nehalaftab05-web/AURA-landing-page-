# landing-page
Responsive product landing page built with pure HTML &amp; CSS. No frameworks. Grid, Flexbox, custom properties, and a CSS animation.
# AURA — Product Landing Page

A responsive product landing page built with pure HTML and CSS. No frameworks, no JavaScript — just clean, intentional markup and layout.

This was built as a frontend practice project to demonstrate real-world page structure: fixed navigation, a hero section, a feature grid using CSS Grid, a specs layout using Flexbox, and a footer. The fictional product is a smart ambient lamp called AURA.

---

## Live Preview

> Open `market.html` directly in any browser — no build step, no dependencies.

---

## What's in it

```
aura-landing-page/
└── index.html       ← the entire project, self-contained
```

All CSS is written inside a `<style>` block in the `<head>`. Google Fonts are loaded via CDN (`Cormorant Garamond` + `Inter`). No external CSS files, no JS libraries.

---

## Page structure

| Section | Purpose | Technique used |
|---|---|---|
| `<nav>` | Fixed top navigation with logo, links, and CTA | `position: fixed`, `backdrop-filter` |
| `.hero` | Full-viewport hero with headline, subtext, and inline SVG lamp | `min-height: 100vh`, CSS keyframe animation |
| `.features` | 3-column feature grid | `CSS Grid` — `grid-template-columns: repeat(3, 1fr)` |
| `.specs` | Two-column specs breakdown | `CSS Flexbox` — `display: flex` with `gap` |
| `.testimonial` | Single pull-quote section | Centered layout, `Cormorant Garamond` italic |
| `.cta-band` | Pre-order call-to-action | Centered text, button styling |
| `<footer>` | Logo, links, copyright | `Flexbox` with `justify-content: space-between` |

---

## Key concepts practiced

- **CSS Grid** for the 3-column feature section (`repeat(3, 1fr)`)
- **CSS Flexbox** for the nav, specs layout, hero actions, and footer
- **CSS custom properties** (`--bg`, `--accent`, `--muted`, etc.) for a consistent design token system
- **Fixed positioning** with `backdrop-filter: blur()` for a glassmorphism navbar
- **CSS keyframe animation** (`@keyframes breathe`) for the hero glow pulse
- **`clamp()`** for fluid typography that scales between viewport sizes
- **Responsive layout** with a single `@media (max-width: 900px)` breakpoint
- **`prefers-reduced-motion`** media query — animation is disabled for users who prefer it
- **Inline SVG** for the lamp illustration and feature icons (no image files needed)
- **Google Fonts via CDN** — `Cormorant Garamond` (display) + `Inter` (body)

---

## Design decisions

The page uses a dark editorial aesthetic — `#0A0A0F` near-black background, warm off-white body text, and a single amber accent (`#E8C97A`) pulled from the product's own world (lamplight). Two typefaces only: a high-contrast serif for headlines and a geometric sans for everything else.

The hero glow animation is the one deliberate design risk — it animates like actual lamplight breathing, slow and ambient. Everything else on the page is quiet.

---

## How to run

```bash
git clone https://github.com/your-username/aura-landing-page.git
cd aura-landing-page
open index.html         # macOS
# or just double-click index.html in your file explorer
```

No installs. No `npm`. No config files.

---

## Screenshot

> *(Add a screenshot here — drag and drop into the GitHub repo's README editor, or use a tool like [Screely](https://screely.com) to create a clean mockup)*

---

## What I'd add next

- Scroll-triggered reveal animations using the Intersection Observer API
- A working email capture form (Formspree or Netlify Forms)
- Dark/light mode toggle
- CSS `:has()` experiments for the feature card hover states
- Semantic improvements: `<main>`, `<article>`, ARIA landmarks

---

## Built with

- HTML5
- CSS3 (Grid, Flexbox, custom properties, animations)
- [Google Fonts](https://fonts.google.com/) — Cormorant Garamond + Inter
- No JavaScript. No frameworks. No build tools.

---

## License

MIT — use it however you like.
