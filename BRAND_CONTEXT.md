# Heartwork Brand Context

**Version:** May 2026
**Status:** Internal
**Use:** Website, marketing copy, decks, proposals, and other client-facing materials.

---

## 1. Brand Summary

Heartwork is a B2B product consultancy.

The brand direction is:

> **Sincere, not sophisticated.**

Heartwork is committed to the work, not the appearance of it. The brand should feel unpretentious, honest, grounded, and genuinely invested in getting things right. It should feel like it is built by people who would rather show something real than something impressive.

The work does the talking.

---

## 2. Brand Personality

### Core qualities

- Sincere
- Committed
- Unpretentious
- Craft-oriented
- Honest
- Observant
- Practical
- Grounded

### What the brand chose

- Authenticity
- Craft
- Honesty
- Clear thinking
- Direct observation
- Useful work over performative polish

### What the brand left behind

- Sophistication for its own sake
- Consulting jargon
- Over-designed polish
- Framework-heavy language
- Impressive-sounding but vague claims
- Brochure-like writing

---

## 3. Positioning Notes

Heartwork should feel like experienced operators working alongside a team, not external consultants delivering a performance.

The brand should communicate:

- We notice what is actually happening.
- We say the thing plainly.
- We work with teams, not above them.
- We care about getting the work right.
- We prefer useful clarity over impressive language.
- We are warm, but not soft.
- We are rigorous, but not performative.

Avoid making the brand feel like:

- A polished agency
- A luxury consultancy
- A wellness brand
- A design studio that values mood over substance
- A corporate transformation firm

---

## 4. Wordmark

### Text

`heartwork`

### Case

All lowercase.

### Tracking

Use wide tracking: approximately `+10%`.

Suggested CSS:

```css
letter-spacing: 0.1em;
```

### Typeface

Use **Zilla Slab** from Google Fonts.

### Style

The whole word leans. Both halves are italic, but `heart` carries more weight than `work`.

- `heart`: Zilla Slab Semibold Italic
- `work`: Zilla Slab Italic

### Meaning

The wordmark should read like a signature more than a conventional logo. It should feel chosen because it felt right, not because it tested well.

It should suggest sincerity, commitment, and craft without becoming overly polished.

### Suggested HTML

```html
<span class="wordmark" aria-label="heartwork">
  <span class="wordmark-heart">heart</span
  ><span class="wordmark-work">work</span>
</span>
```

### Suggested CSS

```css
.wordmark {
  font-family: "Zilla Slab", serif;
  font-style: italic;
  letter-spacing: 0.1em;
  text-transform: lowercase;
}

.wordmark-heart {
  font-weight: 600;
}

.wordmark-work {
  font-weight: 400;
}
```

---

## 5. Colour System

### Primary palette

| Token             | Name       |       Hex | Use                                                                                                  |
| ----------------- | ---------- | --------: | ---------------------------------------------------------------------------------------------------- |
| `--color-primary` | Warm rust  | `#B5533C` | Rules, borders, accents, links, buttons, everyday brand colour                                       |
| `--color-butter`  | Butter     | `#E8D080` | Full-bleed backgrounds, callout panels, card backs. Use at large scale only. Never use as body text. |
| `--color-steel`   | Steel blue | `#2A4A6A` | Data, charts, functional precision, cool counterpoint to rust                                        |
| `--color-dark`    | Dark       | `#1E1610` | Primary dark text and dark backgrounds                                                               |
| `--color-surface` | Surface    | `#F5EFE8` | Main warm page background                                                                            |
| `--color-card`    | Card       | `#FAFAF7` | Cards, raised surfaces, content blocks                                                               |

### Colour character

- **Warm rust** is the main brand colour. It should feel more convicted than terracotta.
- **Butter** creates warmth and mood, but should be used in large fields, not as small functional text.
- **Steel blue** adds tension, precision, and engineering credibility.
- **Dark** should feel warm and grounded, not pure black.
- **Surface** keeps the visual system soft, warm, and human.

### Suggested CSS variables

```css
:root {
  --color-primary: #b5533c;
  --color-butter: #e8d080;
  --color-steel: #2a4a6a;
  --color-dark: #1e1610;
  --color-surface: #f5efe8;
  --color-card: #fafaf7;
}
```

### Accessibility guidance

- Use dark text on surface, card, and butter backgrounds.
- Use surface or card text on dark backgrounds.
- Do not use butter as text.
- Use rust sparingly for emphasis, links, borders, and calls to action.
- Use steel when the design needs structure, technical credibility, data, or contrast.

---

## 6. Typography System

All typefaces are available on Google Fonts.

### Wordmark

- Typeface: **Zilla Slab**
- Use: Logo / wordmark only
- Style: Italic
- Weight: Semibold Italic for `heart`, Italic for `work`

### Headings

- Typeface: **Plus Jakarta Sans**
- Weight: ExtraBold `800`
- Use: H1, H2, H3
- Feel: Modern, clear, structured, confident

### Body

- Typeface: **Inter**
- Weight: Light `300`
- Use: Body copy, descriptive text, paragraphs
- Feel: Quiet, readable, unobtrusive

### Labels / Metadata

- Typeface: **DM Mono**
- Use: Kickers, labels, metadata, captions, hex codes, small utility text
- Feel: Operational, precise, tool-like

### Suggested type scale

| Role         |   Size | Typeface          | Weight |
| ------------ | -----: | ----------------- | -----: |
| H1           | `40px` | Plus Jakarta Sans |    800 |
| H2           | `28px` | Plus Jakarta Sans |    800 |
| H3           | `20px` | Plus Jakarta Sans |    800 |
| Body         | `14px` | Inter             |    300 |
| Small        | `12px` | Inter             |    300 |
| Mono / Label | `11px` | DM Mono           |    400 |

### Suggested Google Fonts import

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link
  href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400&family=Inter:wght@300;400&family=Plus+Jakarta+Sans:wght@800&family=Zilla+Slab:ital,wght@1,400;1,600&display=swap"
  rel="stylesheet"
/>
```

---

## 7. Voice and Writing

### Voice direction

Write like a person who has paid attention.

The writing should be plain, direct, and observant. It should not sound like a consulting brochure. It should not over-explain itself. It should make the work feel concrete.

### Do

- Write plainly.
- Use one idea per sentence.
- Lead with what was observed, not what was concluded.
- Name the thing directly.
- Do not soften what needs to be said.
- Use `we`; this is a partnership, not a service.
- Let the work carry the authority.
- Prefer concrete examples over abstract claims.
- Keep emotional language grounded in real work.

### Do not

- Use consulting jargon.
- Use framework-heavy language.
- Over-qualify or hedge every observation.
- Write to impress.
- Sound like a brochure.
- Make the deck or page more polished than the thinking.
- Stack too many metaphors.
- Drift into poetic language without operational clarity.

### Good writing examples

```text
The team knows what's broken. Nobody has said it yet.
```

```text
Over three weeks of embedded observation, a consistent pattern emerged.
```

```text
Decisions were delayed not by lack of clarity, but by an unspoken fear of naming the obvious.
```

```text
The product team had the answer.
```

```text
The wick was there. It just needed trimming.
```

### Copy style rules

- Prefer short sentences.
- Prefer concrete nouns and verbs.
- Avoid inflated claims.
- Avoid words like `transform`, `unlock`, `synergy`, `innovation`, and `world-class` unless they are genuinely specific and necessary.
- Use warmth, but keep it restrained.
- Use confidence, but do not posture.

---

## 8. Website Guidance

### Overall feel

The website should feel simple, sincere, and useful. It should not feel heavily animated, glossy, or over-designed.

The design should look considered, but not decorated.

### Recommended layout principles

- Use generous whitespace.
- Use warm surfaces.
- Use clear sections.
- Use thin borders and rules in rust or dark with low opacity.
- Use cards sparingly.
- Use butter as a large background or callout surface.
- Use steel for functional contrast or small technical details.
- Avoid gradients unless very subtle.
- Avoid stock imagery.
- Avoid generic SaaS illustrations.
- Avoid excessive icons.

### Buttons

Primary buttons should use warm rust.

Suggested label:

```text
Contact us
```

Suggested email CTA:

```html
<a href="mailto:hello@heartwork.com">Contact us</a>
```

### Link behavior

- Links can use warm rust or steel blue.
- Links should be clearly readable.
- Do not rely only on colour for important states.

---

## 9. Sample CSS Foundation

```css
:root {
  --color-primary: #b5533c;
  --color-butter: #e8d080;
  --color-steel: #2a4a6a;
  --color-dark: #1e1610;
  --color-surface: #f5efe8;
  --color-card: #fafaf7;

  --font-wordmark: "Zilla Slab", serif;
  --font-heading: "Plus Jakarta Sans", sans-serif;
  --font-body: "Inter", sans-serif;
  --font-mono: "DM Mono", monospace;
}

body {
  margin: 0;
  background: var(--color-surface);
  color: var(--color-dark);
  font-family: var(--font-body);
  font-weight: 300;
  font-size: 14px;
  line-height: 1.6;
}

h1,
h2,
h3 {
  font-family: var(--font-heading);
  font-weight: 800;
  line-height: 1.05;
  letter-spacing: -0.03em;
}

h1 {
  font-size: clamp(40px, 8vw, 84px);
}

h2 {
  font-size: clamp(28px, 4vw, 48px);
}

h3 {
  font-size: 20px;
}

.kicker,
.label,
.metadata {
  font-family: var(--font-mono);
  font-size: 11px;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.wordmark {
  font-family: var(--font-wordmark);
  font-style: italic;
  letter-spacing: 0.1em;
  text-transform: lowercase;
}

.wordmark-heart {
  font-weight: 600;
}

.wordmark-work {
  font-weight: 400;
}

.button-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--color-primary);
  color: var(--color-card);
  border: 1px solid var(--color-primary);
  text-decoration: none;
  font-family: var(--font-mono);
  font-size: 11px;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  padding: 0.9rem 1.1rem;
}

.button-primary:hover {
  background: var(--color-dark);
  border-color: var(--color-dark);
}
```

---

## 10. AI / Developer Instructions

When generating website content or UI for Heartwork:

1. Preserve the brand direction: **Sincere, not sophisticated.**
2. Use plain language.
3. Avoid consulting jargon.
4. Use the wordmark treatment exactly: lowercase, italic, Zilla Slab, heavier `heart`, lighter `work`.
5. Use the defined colour tokens. Do not introduce new brand colours unless necessary for accessibility.
6. Use Plus Jakarta Sans for headings, Inter for body, DM Mono for labels, and Zilla Slab for the wordmark.
7. Keep layouts simple, warm, and grounded.
8. Prefer observation-led copy over abstract claims.
9. Avoid making the site feel too polished, glossy, or agency-like.
10. Make the work feel real.

---

## 11. Minimal Brand Tokens

```json
{
  "brand": {
    "name": "Heartwork",
    "wordmark": "heartwork",
    "direction": "Sincere, not sophisticated",
    "description": "A B2B product consultancy committed to the work, not the appearance of it."
  },
  "colors": {
    "primary": "#B5533C",
    "butter": "#E8D080",
    "steel": "#2A4A6A",
    "dark": "#1E1610",
    "surface": "#F5EFE8",
    "card": "#FAFAF7"
  },
  "typefaces": {
    "wordmark": "Zilla Slab",
    "heading": "Plus Jakarta Sans",
    "body": "Inter",
    "label": "DM Mono"
  },
  "wordmarkStyle": {
    "case": "lowercase",
    "tracking": "0.1em",
    "heart": {
      "weight": 600,
      "style": "italic"
    },
    "work": {
      "weight": 400,
      "style": "italic"
    }
  },
  "voice": {
    "do": [
      "Write plainly",
      "Use one idea per sentence",
      "Lead with what was observed",
      "Name the thing directly",
      "Use we",
      "Let the work carry the authority"
    ],
    "dont": [
      "Use consulting jargon",
      "Use framework-heavy language",
      "Over-qualify every observation",
      "Write to impress",
      "Sound like a brochure",
      "Over-polish the presentation"
    ]
  }
}
```
