---
name: cursor-marketing
version: 1.0
last-exported: 2026-08-26

colors:
  primary: "#f54e00"
  primary-active: "#d04200"
  on-primary: "#ffffff"
  ink: "#26251e"
  body: "#5a5852"
  body-strong: "#26251e"
  muted: "#807d72"
  muted-soft: "#a09c92"
  hairline: "#e6e5e0"
  hairline-soft: "#efeee8"
  hairline-strong: "#cfcdc4"
  canvas: "#f7f7f4"
  canvas-soft: "#fafaf7"
  surface-card: "#ffffff"
  surface-strong: "#e6e5e0"
  timeline-thinking: "#dfa88f"
  timeline-grep: "#9fc9a2"
  timeline-read: "#9fbbe0"
  timeline-edit: "#c0a8dd"
  timeline-done: "#c08532"
  semantic-success: "#1f8a65"
  semantic-error: "#cf2d56"

typography:
  display-mega:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "72px"
    fontWeight: "400"
    lineHeight: "1.1"
    letterSpacing: "-2.16px"
  display-lg:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "36px"
    fontWeight: "400"
    lineHeight: "1.2"
    letterSpacing: "-0.72px"
  display-md:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "26px"
    fontWeight: "400"
    lineHeight: "1.25"
    letterSpacing: "-0.325px"
  display-sm:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "22px"
    fontWeight: "400"
    lineHeight: "1.3"
    letterSpacing: "-0.11px"
  title-md:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "18px"
    fontWeight: "600"
    lineHeight: "1.4"
  title-sm:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: "600"
    lineHeight: "1.4"
  body-md:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
  body-tracked:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
    letterSpacing: "0.08px"
  body-sm:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: "400"
    lineHeight: "1.5"
  caption:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "13px"
    fontWeight: "400"
    lineHeight: "1.4"
  eyebrow:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "11px"
    fontWeight: "600"
    lineHeight: "1.4"
    letterSpacing: "0.88px"
    textTransform: "uppercase"
  code:
    fontFamily: "'JetBrains Mono', 'Fira Code', ui-monospace, monospace"
    fontSize: "13px"
    fontWeight: "400"
    lineHeight: "1.5"
  button:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: "500"
    lineHeight: "1"
  nav-link:
    fontFamily: "'CursorGothic', system-ui, 'Helvetica Neue', Helvetica, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: "500"
    lineHeight: "1.4"

rounded:
  none: "0px"
  xs: "4px"
  sm: "6px"
  md: "8px"
  lg: "12px"
  xl: "16px"
  full: "9999px"

spacing:
  xxs: "4px"
  xs: "8px"
  sm: "12px"
  base: "16px"
  md: "20px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
  section: "80px"

layout:
  nav-height: "64px"
  content-max: "1200px"
  section-padding: "80px"
  cta-band-padding: "96px"
  footer-padding: "64px 48px"

components:
  top-nav:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.nav-link}"
    height: "{layout.nav-height}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: "10px 18px"
    height: "40px"
  button-primary-active:
    backgroundColor: "{colors.primary-active}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
  button-secondary:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: "9px 17px"
    height: "40px"
    border: "1px solid {colors.hairline-strong}"
  button-tertiary-text:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
  button-download:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.canvas}"
    typography: "{typography.button}"
    rounded: "{rounded.md}"
    padding: "12px 20px"
    height: "44px"
  hero-band:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.display-mega}"
    padding: "{layout.section-padding}"
  ide-mockup-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    border: "1px solid {colors.hairline}"
    padding: "0"
  ide-pane:
    backgroundColor: "{colors.canvas-soft}"
    textColor: "{colors.body}"
    typography: "{typography.code}"
    rounded: "{rounded.md}"
    padding: "{spacing.base}"
  feature-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.title-md}"
    rounded: "{rounded.lg}"
    border: "1px solid {colors.hairline}"
    padding: "{spacing.lg}"
  comparison-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    border: "1px solid {colors.hairline}"
    padding: "{spacing.lg}"
  testimonial-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.body}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    border: "1px solid {colors.hairline}"
    padding: "{spacing.lg}"
  timeline-pill-thinking:
    backgroundColor: "{colors.timeline-thinking}"
    textColor: "{colors.ink}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  timeline-pill-grep:
    backgroundColor: "{colors.timeline-grep}"
    textColor: "{colors.ink}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  timeline-pill-read:
    backgroundColor: "{colors.timeline-read}"
    textColor: "{colors.ink}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  timeline-pill-edit:
    backgroundColor: "{colors.timeline-edit}"
    textColor: "{colors.ink}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  timeline-pill-done:
    backgroundColor: "{colors.timeline-done}"
    textColor: "{colors.on-primary}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  code-block:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.code}"
    rounded: "{rounded.lg}"
    border: "1px solid {colors.hairline}"
    padding: "{spacing.md}"
  pricing-tier-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    border: "1px solid {colors.hairline}"
    padding: "{spacing.xl}"
  pricing-tier-featured:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.canvas}"
    typography: "{typography.body-md}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xl}"
  text-input:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    border: "1px solid {colors.hairline-strong}"
    padding: "12px 16px"
    height: "44px"
  badge-pill:
    backgroundColor: "{colors.surface-strong}"
    textColor: "{colors.ink}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.full}"
    padding: "4px 10px"
  cta-band:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.display-lg}"
    padding: "{layout.cta-band-padding}"
  footer:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.body}"
    typography: "{typography.body-sm}"
    padding: "{layout.footer-padding}"
  footer-link:
    backgroundColor: "transparent"
    textColor: "{colors.body}"
    typography: "{typography.body-sm}"
---

## Overview

A warm-editorial marketing design system for an AI-first code editor brand. The page floor is **warm cream** (`{colors.canvas}` — #f7f7f4), deliberately not pure white, holding warm near-black ink (`{colors.ink}` — #26251e) for display and body alike. The system runs on **one accent**: `{colors.primary}` (#f54e00) appears exclusively on primary CTAs and the wordmark. Secondary hues never differentiate UI — they are reserved for semantic state and for the product-only timeline palette.

Type uses a single sans family (**CursorGothic**) across display and body, distinguishing hierarchy by size and tracking rather than weight: display sits at weight 400 with negative letter-spacing, titles at 600, body at 400. Every code surface switches to **JetBrains Mono** — and code surfaces occupy roughly half the page.

The signature move is the **AI-timeline pill palette**: five pastels (peach, mint, blue, lavender, gold) marking agent-action stages (Thinking / Grepping / Reading / Editing / Done) inside in-product timeline visualizations. The palette is scoped to those visualizations only and never appears elsewhere in the system.

**Key Characteristics:**

- Warm cream canvas (`{colors.canvas}` — #f7f7f4); ink is warm (#26251e), never pure black.
- Single brand accent (`{colors.primary}` — #f54e00) reserved for primary CTAs and the wordmark. Used scarcely.
- Display weight stays at 400 with negative letter-spacing — an editorial voice, not a bold tech voice.
- Five-token AI-timeline pastel palette, scoped to in-product agent visualizations only.
- Hairline-only depth: 1px borders carry separation. No drop shadows anywhere.
- Compact 8px radius on CTAs and inputs; 12px on cards; 9999px pills for badges and timeline markers.
- 80px section rhythm — generous editorial pacing closer to print than to a SaaS funnel.
- JetBrains Mono on every code surface, including IDE mockup panes.

## Colors

### Brand & Accent

- **Primary** (`{colors.primary}` — #f54e00): The single brand accent. Primary CTA pills, wordmark, hero accents. Used scarcely — scarcity is what gives it voltage.
- **Primary Active** (`{colors.primary-active}` — #d04200): Pressed state for primary CTAs.
- **On Primary** (`{colors.on-primary}` — #ffffff): Text and iconography sitting on the brand orange.

### Surface

- **Canvas** (`{colors.canvas}` — #f7f7f4): The default page floor. Warm cream — the brand differentiator against white-first competitors.
- **Canvas Soft** (`{colors.canvas-soft}` — #fafaf7): IDE-pane backgrounds inside editor mockups.
- **Surface Card** (`{colors.surface-card}` — #ffffff): Card surfaces. Pure white reads as slight elevation against the cream canvas.
- **Surface Strong** (`{colors.surface-strong}` — #e6e5e0): Badge fills and tag pills.
- **Hairline** (`{colors.hairline}` — #e6e5e0): The default 1px border. Same hex family as the canvas, so borders read as one elevation step.
- **Hairline Soft** (`{colors.hairline-soft}` — #efeee8): Lighter internal dividers.
- **Hairline Strong** (`{colors.hairline-strong}` — #cfcdc4): Emphasized outlines — secondary buttons, input borders.

### Text

- **Ink** (`{colors.ink}` — #26251e): Display headlines and emphasized text. Warm near-black.
- **Body Strong** (`{colors.body-strong}` — #26251e): Emphasized running text. Same value as ink.
- **Body** (`{colors.body}` — #5a5852): Default running text, testimonials, footer text.
- **Muted** (`{colors.muted}` — #807d72): Sub-headings and secondary labels.
- **Muted Soft** (`{colors.muted-soft}` — #a09c92): Captions and disabled text.

### Timeline Pastels

Five dedicated tokens for AI-action stages inside in-product timeline visualizations:

- **Thinking** (`{colors.timeline-thinking}` — #dfa88f): Peach pill. Marks the "Thinking" stage.
- **Grepping** (`{colors.timeline-grep}` — #9fc9a2): Mint pill. Marks the "Grepping" stage.
- **Reading** (`{colors.timeline-read}` — #9fbbe0): Pastel-blue pill. Marks the "Reading" stage.
- **Editing** (`{colors.timeline-edit}` — #c0a8dd): Lavender pill. Marks the "Editing" stage.
- **Done** (`{colors.timeline-done}` — #c08532): Warm-gold pill, white label. Marks the "Done" stage.

These are the only multi-hue tokens in the system. They never act as action colors, chart series, or decorative accents outside the timeline context.

### Semantic

- **Success** (`{colors.semantic-success}` — #1f8a65): Confirmation indicators.
- **Error** (`{colors.semantic-error}` — #cf2d56): Validation errors and destructive feedback.

These are the only non-brand, non-timeline hues. They never appear as accents and never drive differentiation.

## Typography

### Font Family

**CursorGothic** is the licensed display and body family. Fallback stack: `system-ui, "Helvetica Neue", Helvetica, Arial, sans-serif`. Code surfaces switch to **JetBrains Mono** with fallback `'Fira Code', ui-monospace, monospace`.

The same family carries display and body — hierarchy comes from size, weight, and tracking, not from a second face. Display runs at weight 400 with negative letter-spacing (-0.11px to -2.16px); titles run at 600; body stays at 400. The eyebrow (`{typography.eyebrow}`, 11px uppercase) is the only uppercase role.

### Hierarchy

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---|---|---|---|---|
| `{typography.display-mega}` | 72px | 400 | 1.1 | -2.16px | Homepage hero headline |
| `{typography.display-lg}` | 36px | 400 | 1.2 | -0.72px | Section heads, CTA bands |
| `{typography.display-md}` | 26px | 400 | 1.25 | -0.325px | Sub-section heads |
| `{typography.display-sm}` | 22px | 400 | 1.3 | -0.11px | Card group titles |
| `{typography.title-md}` | 18px | 600 | 1.4 | 0 | Feature card titles |
| `{typography.title-sm}` | 16px | 600 | 1.4 | 0 | List labels |
| `{typography.body-md}` | 16px | 400 | 1.5 | 0 | Default running text |
| `{typography.body-tracked}` | 16px | 400 | 1.5 | +0.08px | Tracked editorial body |
| `{typography.body-sm}` | 14px | 400 | 1.5 | 0 | Footer body, nav links |
| `{typography.caption}` | 13px | 400 | 1.4 | 0 | Photo captions |
| `{typography.eyebrow}` | 11px | 600 | 1.4 | +0.88px, uppercase | Section labels, pill labels |
| `{typography.code}` | 13px | 400 | 1.5 | 0 | Mono: code blocks, IDE panes |
| `{typography.button}` | 14px | 500 | 1.0 | 0 | Button labels |
| `{typography.nav-link}` | 14px | 500 | 1.4 | 0 | Top navigation |

### Principles

Display weights stay at 400 — the editorial voice depends on it, and the system never reaches for 700+. Negative letter-spacing is reserved for display sizes; body sizes run zero or near-zero tracking. Mono type appears only on code-adjacent surfaces (code blocks, inline code, IDE panes) and never replaces sans body text.

### Note on Font Substitutes

CursorGothic is licensed. The closest open substitute is **Inter** at weight 400 with letter-spacing reduced roughly 1.5% to preserve the tight display feel. Avoid substituting a high-contrast serif — it breaks the system's engineering-editorial balance.

## Layout

### Spacing System

- **Base unit:** 4px.
- **Tokens:** `{spacing.xxs}` 4px · `{spacing.xs}` 8px · `{spacing.sm}` 12px · `{spacing.base}` 16px · `{spacing.md}` 20px · `{spacing.lg}` 24px · `{spacing.xl}` 32px · `{spacing.xxl}` 48px · `{spacing.section}` 80px.
- **Section padding:** `{layout.section-padding}` (80px) — the editorial rhythm.
- **Card internal padding:** `{spacing.lg}` (24px) for feature and comparison cards; `{spacing.xl}` (32px) for pricing tiers.
- **CTA band padding:** `{layout.cta-band-padding}` (96px) — the most generous vertical space in the system.

### Grid & Container

- **Max content width:** `{layout.content-max}` (1200px).
- **Feature card grids:** 2-up for split/comparison layouts, 3-up for benefit rows.
- **Footer:** 5-column link grid at desktop.
- **Top navigation:** `{layout.nav-height}` (64px), wordmark left, menu center-right, sign-in + download right.

### Whitespace Philosophy

Generous editorial pacing — closer to a print magazine than a tech site. Sections breathe at 80px while cards inside a band sit close together at 16–24px gaps. The tension between airy sections and tight card clusters is intentional: it keeps the page calm without feeling empty.

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| Flat (canvas) | `{colors.canvas}` background, no border | Body bands, hero, CTA band, footer |
| Card | `{colors.surface-card}` background + 1px `{colors.hairline}` border | Content cards, pricing tiers, code blocks |
| Pane | `{colors.canvas-soft}` background inside cards | IDE mockup panes |
| Pill | Full-radius fill | Badges, tags, timeline pills |

The elevation philosophy is **hairline-only depth**. There are no shadow tokens: cards float above the canvas through the white-on-cream contrast and a 1px border. The IDE-mockup card is the only composition with internal layered structure — sidebar, editor, chat panel, terminal — mimicking the real product shell.

## Shapes

### Border Radius Scale

| Token | Value | Use |
|---|---|---|
| `{rounded.none}` | 0px | Reserved |
| `{rounded.xs}` | 4px | Inline tags |
| `{rounded.sm}` | 6px | Compact rows |
| `{rounded.md}` | 8px | CTA buttons, form inputs |
| `{rounded.lg}` | 12px | Cards, IDE mockups, code blocks |
| `{rounded.xl}` | 16px | Large feature cards (rare) |
| `{rounded.full}` | 9999px | Pills, badges, avatars |

The radius ladder is hierarchical: interactive controls sit at 8px, containers at 12px, pills at 9999px. Don't mix levels within one component.

## Components

### Top Navigation

**`top-nav`** — Background `{colors.canvas}`, text `{colors.ink}`, height `{layout.nav-height}` (64px). Carries the wordmark left, the primary horizontal menu (Pricing / Features / Enterprise / Blog / Forum / Careers), and a right cluster with Sign In plus a `button-primary` download CTA.

### Buttons

**`button-primary`** — The signature orange CTA. Background `{colors.primary}`, text `{colors.on-primary}`, type `{typography.button}` (14px / 500), height 40px, padding 10px × 18px, rounded `{rounded.md}` (8px). Pressed state darkens to `{colors.primary-active}`.

**`button-secondary`** — White pill on cream canvas. Background `{colors.surface-card}`, text `{colors.ink}`, 1px `{colors.hairline-strong}` border, same height and radius as primary.

**`button-tertiary-text`** — Inline ink text link for low-emphasis actions.

**`button-download`** — The large ink-on-cream CTA. Background `{colors.ink}`, text `{colors.canvas}`, height 44px, padding 12px × 20px. Reserved for platform download actions.

### Hero & IDE Mockups

**`hero-band`** — Background `{colors.canvas}`, display headline in `{typography.display-mega}` (72px / 400 / -2.16px), subhead in `{typography.body-md}`, and a CTA pair of `button-download` + `button-tertiary-text`. An `ide-mockup-card` sits centered below the copy.

**`ide-mockup-card`** — White card containing a multi-pane editor mockup (sidebar + main editor + chat panel + terminal). Background `{colors.surface-card}`, rounded `{rounded.lg}`, 1px `{colors.hairline}` border, zero padding — panes fill edge-to-edge.

**`ide-pane`** — A single pane inside the mockup. Background `{colors.canvas-soft}`, text `{colors.body}` in `{typography.code}`, rounded `{rounded.md}`, padding `{spacing.base}`.

### Cards

**`feature-card`** — Background `{colors.surface-card}`, title in `{typography.title-md}`, rounded `{rounded.lg}`, 1px `{colors.hairline}` border, padding `{spacing.lg}`.

**`comparison-card`** — Side-by-side product-comparison card. Same surface treatment; internally split into two columns.

**`testimonial-card`** — Quote card. Background `{colors.surface-card}`, text `{colors.body}`, rounded `{rounded.lg}`, padding `{spacing.lg}`.

### AI Timeline Pills

Five pill variants mark agent-action stages inside in-product timeline visualizations. All share shape and type — `{typography.eyebrow}` (11px / 600 / +0.88px tracking, uppercase), `{rounded.full}`, padding 4px × 10px — and differ only by fill:

- **`timeline-pill-thinking`** — Peach fill (`{colors.timeline-thinking}`), ink label.
- **`timeline-pill-grep`** — Mint fill (`{colors.timeline-grep}`), ink label.
- **`timeline-pill-read`** — Pastel-blue fill (`{colors.timeline-read}`), ink label.
- **`timeline-pill-edit`** — Lavender fill (`{colors.timeline-edit}`), ink label.
- **`timeline-pill-done`** — Gold fill (`{colors.timeline-done}`), white label.

### Code

**`code-block`** — Background `{colors.surface-card}`, text `{colors.ink}` in `{typography.code}`, rounded `{rounded.lg}`, 1px `{colors.hairline}` border, padding `{spacing.md}`.

### Pricing

**`pricing-tier-card`** — Background `{colors.surface-card}`, rounded `{rounded.lg}`, 1px `{colors.hairline}` border, padding `{spacing.xl}`.

**`pricing-tier-featured`** — Featured tier inverts to ink: background `{colors.ink}`, text `{colors.canvas}`. Dark inversion signals emphasis without a colored ribbon.

### Forms & Tags

**`text-input`** — Background `{colors.surface-card}`, text `{colors.ink}`, rounded `{rounded.md}`, 1px `{colors.hairline-strong}` border, padding 12px × 16px, height 44px.

**`badge-pill`** — Uppercase tag pill. Background `{colors.surface-strong}`, text `{colors.ink}`, type `{typography.eyebrow}`, rounded `{rounded.full}`, padding 4px × 10px.

### CTA Band & Footer

**`cta-band`** — Pre-footer conversion band. Background `{colors.canvas}`, centered display headline in `{typography.display-lg}`, a single `button-primary`. Vertical padding `{layout.cta-band-padding}` (96px).

**`footer`** — Closing footer. Background `{colors.canvas}`, text `{colors.body}`, 5-column link grid, padding `{layout.footer-padding}` (64px × 48px).

**`footer-link`** — Transparent background, text `{colors.body}`, type `{typography.body-sm}`.

## Do's and Don'ts

### Do

- Anchor every page on `{colors.canvas}` (#f7f7f4). Pure white reads as generic SaaS; the cream floor is the brand.
- Reserve `{colors.primary}` (#f54e00) for primary CTAs and the wordmark. Scarcity is the point.
- Keep display weight at 400 with negative tracking. The editorial voice depends on it.
- Render every code surface — inline, blocks, IDE panes — in `{typography.code}` (JetBrains Mono).
- Carry depth with 1px `{colors.hairline}` borders and surface contrast.
- Scope the five timeline pastels to in-product agent visualizations.
- Use the radius ladder: 8px controls, 12px containers, 9999px pills.

### Don't

- Don't introduce a second brand action color. `{colors.primary}` is the only one.
- Don't bold display text past 400. Titles cap at 600.
- Don't add drop shadows or glow effects. Hairlines carry all depth.
- Don't reuse timeline pastels as system action colors, chart series, or decoration.
- Don't place cool grays or pure-white page backgrounds on the canvas. Warm tones only.
- Don't sample colors from third-party embeds (cookie consent, widgets). Only tokens in this document are authoritative.

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 640px | Hero drops to 32px h1; IDE mockup collapses to a single pane preview; feature grid 1-up; nav becomes hamburger |
| Tablet | 640–1024px | Hero at 56px; IDE mockup compresses; feature grid 2-up |
| Desktop | 1024–1280px | Full 72px hero; full multi-pane IDE mockup; feature grid 3-up |
| Wide | > 1280px | Content caps at `{layout.content-max}` (1200px) |

### Touch Targets

- `button-primary` at 40px height meets WCAG AA; padded area approaches AAA.
- `button-download` and `text-input` at 44px height meet WCAG AAA.
- `top-nav` links render at 14px with generous hit spacing around each item.

### Collapsing Strategy

- Top nav switches to hamburger below 768px.
- The IDE mockup reduces to a single primary pane on mobile rather than scaling all four panes down.
- Feature grids step down 3-up → 2-up → 1-up; display type steps down 72px → 56px → 32px instead of shrinking proportionally.

## Iteration Guide

1. **Focus on ONE component at a time.** Reference its YAML key (`{component.button-primary}`, `{component.ide-mockup-card}`).
2. **Variants live as separate entries** under `components:` (`-active`, `-featured`). Don't merge states into one entry.
3. **Use `{token.refs}` everywhere** — never inline hex. Inline hex is implementation drift.
4. **Document Default and Pressed states only.** Hover is intentionally unspecified; don't invent tones beyond `{colors.primary-active}`.
5. **Display stays 400 with negative tracking; titles cap at 600.** The split is unbreakable.
6. **Orange stays scarce.** If a second orange element appears on screen next to a primary CTA, one of them is wrong.
7. **Timeline pastels stay scoped** to in-product agent visualizations.
8. **When in doubt, add whitespace before adding color.** The system communicates through pacing, not hue count.

## Known Gaps

- CursorGothic is licensed; Inter is the informal substitute and is not formalized as a fallback token here.
- Motion timings (timeline pill entrance, IDE pane reveal, scroll transitions) are out of scope for this export.
- In-app surfaces (editor chrome, chat panel, command bar) are captured only indirectly via the marketing IDE mockup.
- Form validation states beyond focus are documented narratively but not extracted as component entries.
- Iconography (stroke width, grid, sizing) is not tokenized yet.

---

## Appendix A — Token Quick Reference

```css
/* Brand */
--color-primary: #f54e00;
--color-primary-active: #d04200;
--color-on-primary: #ffffff;

/* Surface */
--color-canvas: #f7f7f4;
--color-canvas-soft: #fafaf7;
--color-surface-card: #ffffff;
--color-surface-strong: #e6e5e0;
--color-hairline: #e6e5e0;
--color-hairline-soft: #efeee8;
--color-hairline-strong: #cfcdc4;

/* Ink */
--color-ink: #26251e;
--color-body: #5a5852;
--color-body-strong: #26251e;
--color-muted: #807d72;
--color-muted-soft: #a09c92;

/* Timeline pastels */
--color-timeline-thinking: #dfa88f;
--color-timeline-grep: #9fc9a2;
--color-timeline-read: #9fbbe0;
--color-timeline-edit: #c0a8dd;
--color-timeline-done: #c08532;

/* Semantic */
--color-success: #1f8a65;
--color-error: #cf2d56;

/* Radius */
--radius-none: 0px;
--radius-xs: 4px;
--radius-sm: 6px;
--radius-md: 8px;
--radius-lg: 12px;
--radius-xl: 16px;
--radius-full: 9999px;

/* Spacing */
--space-xxs: 4px;
--space-xs: 8px;
--space-sm: 12px;
--space-base: 16px;
--space-md: 20px;
--space-lg: 24px;
--space-xl: 32px;
--space-xxl: 48px;
--space-section: 80px;

/* Layout */
--layout-nav-height: 64px;
--layout-content-max: 1200px;
--layout-section-padding: 80px;
--layout-cta-band-padding: 96px;
--layout-footer-padding: 64px 48px;

/* Type families */
--font-sans: "CursorGothic", system-ui, "Helvetica Neue", Helvetica, Arial, sans-serif;
--font-mono: "JetBrains Mono", "Fira Code", ui-monospace, monospace;
```
