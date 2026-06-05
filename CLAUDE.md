# Heartwork Website

Marketing site for Heartwork — a B2B embedded product team consultancy.

## Structure

Single-page static site (`index.html`). No build step, no framework, no dependencies beyond Google Fonts. CSS lives inline in `<style>` in the `<head>`. JS is minimal, inline at the bottom.

## Deployment

GitHub Pages. Custom domain: `heartwork.in` (set via `CNAME`). Pushes to `main` deploy automatically.

## Brand

`BRAND_CONTEXT.md` is the source of truth for all visual and voice decisions. Read it before making any copy or design changes.

Key constraints from it:
- Brand direction: **Sincere, not sophisticated.**
- Avoid consulting jargon, over-polish, agency language, and abstract claims.
- Write plainly. One idea per sentence. Lead with observation, not conclusion.
- Use `we` — this is a partnership.

### Colour tokens

| Token       | Hex       | Use                                      |
|-------------|-----------|------------------------------------------|
| `--rust`    | `#B5533C` | Primary brand — accents, links, buttons  |
| `--butter`  | `#E8D080` | Large backgrounds and callout panels only |
| `--steel`   | `#2A4A6A` | Functional contrast, data, precision     |
| `--dark`    | `#1E1610` | Primary dark text and dark backgrounds   |
| `--surface` | `#F5EFE8` | Main warm page background                |
| `--care`    | `#FAFAF7` | Cards and raised surfaces (`--color-card` in brand doc) |

### Typefaces (Google Fonts)

- **Wordmark:** Zilla Slab — italic, semibold (`700`) for `heart`, regular (`400`) for `work`
- **Headings:** Plus Jakarta Sans — ExtraBold `800`
- **Body:** Inter — Light `300`
- **Labels / metadata / mono:** DM Mono — `400`

### Wordmark HTML pattern

```html
<span class="wordmark">
  <span class="wordmark-logo"></span>
  <span class="bold">heart</span><span class="light-wt">work</span>
</span>
```

All lowercase. Wide tracking (`0.1em`). Never change the weight split between `heart` and `work`.

## Page sections (top to bottom)

1. **Nav** — fixed, transitions: transparent → dark (scrolled in hero) → light (past hero)
2. **Hero** — dark background, eyebrow + H1 + sub + CTA
3. **Pain** — recognition quotes + problem framing (`#about`)
4. **Services** — four service cards in a 2×2 grid (`#services`)
5. **How** — three-stage process on dark background (`#how`)
6. **Stats** — track record numbers (`#track-record`)
7. **Who** — who we help + aside (`who`)
8. **Team** — Aarti Bhatnagar (Research & Design) and Hari Mohanraj (Engineering & Product)
9. **Contact** — CTA on dark background (`#contact`), email: `hello@heartwork.in`
10. **Footer**

## Working conventions

- Edit `index.html` directly — it's the whole site.
- Do not introduce a build tool, bundler, or framework unless explicitly asked.
- Do not add new Google Fonts families. Use the four already loaded.
- Do not introduce new brand colours. Extend via opacity variants of existing tokens if needed.
- Keep CSS inline. Keep JS minimal and inline.
- Test responsiveness — the breakpoint is `768px`; mobile hides nav links and collapses grids to single column.
