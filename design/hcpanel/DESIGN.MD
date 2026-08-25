---
name: design-system
version: 1.0
last-exported: 2026-08-24

colors:
  primary: "#145fe4"
  primary-hover: "#0e55d1"
  primary-active: "#0d4fc3"
  primary-soft: "rgba(20, 95, 228, 0.08)"
  primary-soft-hover: "rgba(20, 95, 228, 0.14)"
  primary-soft-dark: "rgba(20, 95, 228, 0.15)"
  on-primary: "#ffffff"
  canvas: "#f6f8fb"
  surface: "#ffffff"
  surface-soft: "#f4f6f9"
  surface-hover: "#eceff3"
  hairline: "#e6e9ee"
  hairline-strong: "#d5dae1"
  ink: "#1d1d21"
  ink-secondary: "#3f434b"
  muted: "#67707c"
  ink-faint: "#9aa3af"
  success: "#18794e"
  danger: "#d1242f"
  warning: "#b45309"
  # Dark theme
  canvas-dark: "#010102"
  surface-dark: "#0f1011"
  surface-dark-soft: "#141516"
  surface-dark-hover: "#18191a"
  hairline-dark: "#23252a"
  hairline-dark-strong: "#34343a"
  ink-dark: "#f7f8f8"
  ink-dark-secondary: "#d0d6e0"
  muted-dark: "#8a8f98"
  ink-faint-dark: "#62666d"
  success-dark: "#27a644"
  danger-dark: "#ff6b74"
  warning-dark: "#e8923c"

typography:
  display:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "40px"
    fontWeight: "600"
    lineHeight: "1.15"
    letterSpacing: "-0.01em"
  h1:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "24px"
    fontWeight: "600"
    lineHeight: "1.25"
  h2:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "18px"
    fontWeight: "600"
    lineHeight: "1.3"
  h3:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "15px"
    fontWeight: "600"
    lineHeight: "1.35"
  title:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "16px"
    fontWeight: "500"
    lineHeight: "1.4"
  body:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "14px"
    fontWeight: "400"
    lineHeight: "1.5"
  body-sm:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "13px"
    fontWeight: "400"
    lineHeight: "1.5"
  button:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "14px"
    fontWeight: "600"
    lineHeight: "1"
  caption:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "12px"
    fontWeight: "400"
    lineHeight: "1.4"
  eyebrow:
    fontFamily: "system-ui, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, sans-serif"
    fontSize: "11px"
    fontWeight: "600"
    lineHeight: "1.4"
    letterSpacing: "0.5px"
    textTransform: "uppercase"
  code:
    fontFamily: "ui-monospace, SFMono-Regular, SF Mono, Menlo, Consolas, monospace"
    fontSize: "13px"
    fontWeight: "400"
    lineHeight: "1.6"

rounded:
  xs: "2px"
  sm: "4px"
  md: "6px"
  lg: "8px"
  xl: "12px"
  full: "9999px"

spacing:
  xxs: "4px"
  xs: "8px"
  sm: "12px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
  section: "64px"

motion:
  fast: "100ms"
  base: "300ms"
  slow: "500ms"
  ease: "cubic-bezier(0.4, 0, 0.2, 1)"

layout:
  sidebar-width: "244px"
  topbar-height: "64px"
  content-max: "2560px"
  content-padding: "32px"
  card-padding: "24px"
  section-padding: "64px"

components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    height: "36px"
    padding: "0 16px"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
  button-primary-active:
    backgroundColor: "{colors.primary-active}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    height: "36px"
    padding: "0 16px"
    border: "1px solid {colors.hairline}"
  button-utility:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    border: "1px solid {colors.hairline}"
  button-danger:
    backgroundColor: "{colors.danger}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    height: "36px"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    border: "1px solid {colors.hairline}"
    shadow: "0 1px 2px rgba(15,17,21,.04), 0 1px 3px rgba(15,17,21,.04)"
    padding: "{spacing.lg}"
  card-elevated:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    shadow: "0 2px 4px rgba(15,17,21,.04), 0 8px 24px rgba(15,17,21,.08)"
  card-modal:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    shadow: "0 8px 24px rgba(15,17,21,.10), 0 24px 64px rgba(15,17,21,.16)"
  stat-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    typography: "{typography.title}"
    rounded: "{rounded.md}"
    border: "1px solid {colors.hairline}"
    padding: "{spacing.lg}"
  nav-link:
    backgroundColor: "transparent"
    textColor: "{colors.ink-secondary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "10px 12px"
  nav-link-active:
    backgroundColor: "transparent"
    textColor: "{colors.primary}"
    typography: "{typography.body}"
    accentBar: "3px solid {colors.primary} (left, ::before)"
  text-input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    border: "1px solid {colors.hairline}"
    padding: "8px 12px"
  text-input-focused:
    border: "1px solid {colors.primary}"
    ring: "0 0 0 3px {colors.primary-soft}"
  toast-success:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    accentBar: "4px solid {colors.success}"
    rounded: "{rounded.md}"
    shadow: "0 2px 4px rgba(15,17,21,.04), 0 8px 24px rgba(15,17,21,.08)"
  toast-danger:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    accentBar: "4px solid {colors.danger}"
    rounded: "{rounded.md}"
  toast-info:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    accentBar: "4px solid {colors.primary}"
    rounded: "{rounded.md}"
  table-data:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    border: "hairline horizontal between rows"
    headerTypography: "{typography.eyebrow}"
    rowHover: "{colors.surface-hover}"
  sidebar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    width: "{layout.sidebar-width}"
    border: "1px solid {colors.hairline} (right)"
  topbar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    height: "{layout.topbar-height}"
    border: "1px solid {colors.hairline} (bottom)"
  badge-eyebrow:
    backgroundColor: "{colors.primary-soft}"
    textColor: "{colors.primary}"
    typography: "{typography.eyebrow}"
    rounded: "{rounded.xs}"
    padding: "2px 8px"
---

## Overview

A single-accent control-panel design system. The default canvas is a tinted near-white (`{colors.canvas}` — #f6f8fb) — cool enough to feel like a working tool, warm enough to read as light. The brand voltage comes from **one accent, used everywhere**: `{colors.primary}` (#145fe4) appears on buttons, links, focus rings, navigation active state, eyebrows, and the brand mark. Secondary hues are reserved exclusively for state — `success` for green confirmations, `danger` for destructive, `warning` for caution — never for differentiation.

The system has two surface modes:

1. **Light canvas** (`{colors.canvas}` + `{colors.surface}`) — the default. `{colors.canvas}` is the page floor; `{colors.surface}` (pure white) is the card surface.
2. **Dark canvas** (`{colors.canvas-dark}` — #010102) — near-black, with charcoal `{colors.surface-dark}` cards. Dark mode inverts the ink scale to `{colors.ink-dark}` while keeping the brand blue identical.

The signature move is **monochromatic charts**. We never ship a multi-color product palette; the 8-step blue ramp from `{colors.primary}` (#145fe4) down to `#0a3a8c` (deepest) and up to `#cfe0ff` (lightest) handles every service-distribution, intensity, and magnitude chart. State-mix donuts use a separate outcome palette (blue / green / amber / violet / red / teal) but that palette is scoped to those charts only.

**Key Characteristics:**

- Single brand accent (`{colors.primary}` — #145fe4) used on every primary action, link, and active state. No secondary brand colors in product UI.
- Light canvas (`{colors.canvas}` — #f6f8fb) with hairline borders (`{colors.hairline}` — #e6e9ee) — the working-tool aesthetic, not the marketing-page aesthetic.
- Dark canvas (`{colors.canvas-dark}` — #010102) with charcoal surfaces (`{colors.surface-dark}` — #0f1011). Inverts ink to `{colors.ink-dark}` (#f7f8f8). Brand blue unchanged.
- Flat elevation. Three shadow tokens (`--shadow-card`, `--shadow-elevated`, `--shadow-modal`) — no neobrutalism, no glow.
- System font stack only — no webfonts. Inter, system-ui, and SF Mono substitutes are acceptable.
- 8-step monochromatic blue palette for every intensity / service chart.
- Motion is restrained: 100ms hover, 300ms color transitions, 500ms entrance. No spring physics.
- Sidebar nav at 244px, topbar at 64px, content max 2560px with 32px padding.
- Restrained radius scale: 4px buttons/inputs, 6px cards, 8px modals, 9999px pills.

## Colors

### Brand & Accent

- **Primary** (`{colors.primary}` — #145fe4): The signature brand blue. Used on every primary CTA background, links, focus rings, eyebrows, navigation active state, and brand mark. The single accent that carries the system.
- **Primary Hover** (`{colors.primary-hover}` — #0e55d1): One tone darker. Applied on `:hover` for primary buttons.
- **Primary Active** (`{colors.primary-active}` — #0d4fc3): Two tones darker. Applied on `:active` (pressed) state.
- **Primary Soft** (`{colors.primary-soft}` — rgba(20, 95, 228, 0.08)): The faint brand tint used as a focus-ring background, badge fill, and selected-state tint.
- **Primary Soft Hover** (`{colors.primary-soft-hover}` — rgba(20, 95, 228, 0.14)): A deeper soft variant for hover on tinted backgrounds.
- **On Primary** (`{colors.on-primary}` — #ffffff): All text and iconography sitting on the brand blue. AA contrast passes against `{colors.primary}`.

### Surface

- **Canvas** (`{colors.canvas}` — #f6f8fb): The default page floor. Cool near-white — the working-tool tone, deliberately not pure white.
- **Surface** (`{colors.surface}` — #ffffff): Card backgrounds, modal surfaces, input backgrounds, table backgrounds. Pure white sits on top of the canvas tint.
- **Surface Soft** (`{colors.surface-soft}` — #f4f6f9): Section dividers, very-soft band backgrounds, alternating table row tint.
- **Surface Hover** (`{colors.surface-hover}` — #eceff3): Hover state for rows, nav items, and secondary buttons on light canvas.
- **Hairline** (`{colors.hairline}` — #e6e9ee): The 1px border tone. Same hex family as canvas; borders read as one elevation step.
- **Hairline Strong** (`{colors.hairline-strong}` — #d5dae1): A slightly stronger border for emphasized separation (e.g. modal backdrop edges).

#### Dark Theme Surfaces

- **Canvas Dark** (`{colors.canvas-dark}` — #010102): Near-black page floor. Slightly off-pure-black for warmth.
- **Surface Dark** (`{colors.surface-dark}` — #0f1011): Dark cards, sidebar, topbar, modals — one step lighter than canvas.
- **Surface Dark Soft** (`{colors.surface-dark-soft}` — #141516): Dark section dividers and soft bands.
- **Surface Dark Hover** (`{colors.surface-dark-hover}` — #18191a): Hover state on dark canvas.
- **Hairline Dark** (`{colors.hairline-dark}` — #23252a): Dark-mode 1px border.
- **Hairline Dark Strong** (`{colors.hairline-dark-strong}` — #34343a): Dark-mode emphasized border.
- **Primary Soft Dark** (`{colors.primary-soft-dark}` — rgba(20, 95, 228, 0.15)): Dark-mode brand tint. Stronger alpha than light mode because dark backgrounds eat translucency.

### Text

- **Ink** (`{colors.ink}` — #1d1d21): All primary text and headlines. Warm near-black.
- **Ink Secondary** (`{colors.ink-secondary}` — #3f434b): Body text, labels, secondary nav items.
- **Muted** (`{colors.muted}` — #67707c): Sub-headings, helper text, footer-adjacent text.
- **Ink Faint** (`{colors.ink-faint}` — #9aa3af): Captions, fine-print, disabled text.
- **On Dark** (dark mode `{colors.ink-dark}` — #f7f8f8): Primary text on dark surfaces.
- **On Dark Secondary** (`{colors.ink-dark-secondary}` — #d0d6e0): Secondary text on dark surfaces.
- **Muted Dark** (`{colors.muted-dark}` — #8a8f98): Muted text in dark mode.
- **Ink Faint Dark** (`{colors.ink-faint-dark}` — #62666d): Disabled text in dark mode.

### Semantic

- **Success** (`{colors.success}` — #18794e): Confirmations, ban-list successful operations, successful auth. Dark variant `{colors.success-dark}` — #27a644.
- **Danger** (`{colors.danger}` — #d1242f): Destructive actions, errors, failed auth. Dark variant `{colors.danger-dark}` — #ff6b74.
- **Warning** (`{colors.warning}` — #b45309): Caution toasts, attention-needed states. Dark variant `{colors.warning-dark}` — #e8923c.

These are the only non-brand hues in the system. They never appear as accents, never drive chart series, never paint product UI surfaces.

## Typography

### Font Family

The system uses a **system font stack** — no webfonts, no licensing. Sans: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif`. Mono: `ui-monospace, SFMono-Regular, "SF Mono", Menlo, Consolas, "Liberation Mono", monospace` — used in IP tables, code columns, audit logs, and code snippets. Inter is an acceptable substitute for the sans stack because of its similar humanist proportions.

The system uses the same family for display and body — distinguishing hierarchy by **size and weight**, not face. Display sizes run 40px / 600; body sizes run 14px / 400. The eyebrow (`{typography.eyebrow}`) is the only uppercase role, used sparingly as a label-anchor inside cards.

### Hierarchy

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---|---|---|---|---|
| `{typography.display}` | 40px | 600 | 1.15 | -0.01em | Hero numbers, page-anchoring metrics |
| `{typography.h1}` | 24px | 600 | 1.25 | 0 | Page titles |
| `{typography.h2}` | 18px | 600 | 1.3 | 0 | Card titles, section heads |
| `{typography.h3}` | 15px | 600 | 1.35 | 0 | Sub-section heads, list-section titles |
| `{typography.title}` | 16px | 500 | 1.4 | 0 | List-item titles, stat values |
| `{typography.body}` | 14px | 400 | 1.5 | 0 | Default running text, table cells |
| `{typography.body-sm}` | 13px | 400 | 1.5 | 0 | Helper text, dense table cells |
| `{typography.button}` | 14px | 600 | 1.0 | 0 | All button labels |
| `{typography.caption}` | 12px | 400 | 1.4 | 0 | Captions, chart axis labels |
| `{typography.eyebrow}` | 11px | 600 | 1.4 | +0.5px, uppercase | Card labels, nav section labels, table headers |
| `{typography.code}` | 13px | 400 | 1.6 | 0 | Mono: IP tables, audit logs, code |

### Principles

Display and heading weights stay at 600 — the system never bolds beyond that. Body weights stay at 400 (paragraphs) and 500 (titles). Negative letter-spacing is reserved for `{typography.display}` (-0.01em); smaller sizes run zero tracking because the system stack is already tight at 14-16px.

Eyebrow text is the only uppercase role. It anchors sections inside cards (`.eyebrow` directly above the `<h2>`) and labels table headers. Eyebrows never end with punctuation.

Mono type (`{typography.code}`) appears only in code-adjacent contexts: IP addresses in tables, audit log entries, hex codes in developer pages. It never replaces sans body text.

### Note on Font Substitutes

The system stack is system-font only, so no licensing concerns. If a project needs a custom face: **Inter** is the closest humanist sans substitute for the system stack; **IBM Plex Sans** works too. For mono, **JetBrains Mono** is the closest substitute to the SF Mono / Menlo stack.

## Layout

### Spacing System

- **Base unit:** 4px.
- **Tokens:** `{spacing.xxs}` 4px · `{spacing.xs}` 8px · `{spacing.sm}` 12px · `{spacing.md}` 16px · `{spacing.lg}` 24px · `{spacing.xl}` 32px · `{spacing.xxl}` 48px · `{spacing.section}` 64px.
- **Section padding:** `{spacing.section}` (64px) — the working-tool rhythm, more compact than SaaS marketing.
- **Card internal padding:** `{spacing.lg}` (24px) for cards and stat tiles; `{spacing.xl}` (32px) for hero cards.
- **Modal padding:** `{spacing.xl}` (32px).
- **Grid gutters:** `{spacing.lg}` (24px).

### Grid & Container

- **Max content width:** `{layout.content-max}` (2560px) — wide enough for ultra-wide monitors; in practice most pages sit inside 1200-1600px.
- **Sidebar:** `{layout.sidebar-width}` (244px) fixed-left.
- **Topbar:** `{layout.topbar-height}` (64px) fixed-top.
- **Content padding:** `{layout.content-padding}` (32px) on the main column.

### Common Grids

- **`.grid-stats`** — `repeat(auto-fit, minmax(220px, 1fr))` for top-of-page stat cards. Collapses to 2-up at 960px, 1-up at 640px.
- **`.grid-two-col`** — Two equal columns, collapses to one below 960px.
- **`.grid-settings`** / **`.grid-settings-wide`** — Two columns with optional full-width span. Used for forms.
- **`.grid-three-up`** — Three equal columns for content cards; collapses to 1-up at 768px.

### Whitespace Philosophy

The light canvas + hairline borders + restrained type create a working-tool pacing — closer to a control panel than a marketing page. Whitespace between cards stays uniform at `{spacing.lg}` (24px); whitespace between sections stays at `{spacing.xl}` (32px). Internal card padding is generous at 24px so type and data have room to breathe without feeling sparse.

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| Flat | No shadow, no border | Body sections, top nav, hero bands |
| Hairline | 1px `{colors.hairline}` border | Cards, inputs, sub-nav, table rows |
| Card | `{colors.surface}` background + `{colors.hairline}` border + `{shadow.card}` | Default page blocks |
| Elevated | `{shadow.elevated}` — no border | Hover state on cards, dropdown menus |
| Modal | `{shadow.modal}` — no border | Modals, popovers, command palettes |
| Focus ring | `{shadow.focus}` — 3px `{colors.primary-soft}` outer ring | All focusable elements on focus |

The elevation philosophy is **hairline first, shadow second**. Cards gain depth from a 1px border, not a drop shadow. Shadow is reserved for hover-lift and modal layering. Dark theme replaces the rgba shadows with deeper black equivalents (rgba(0,0,0,0.3) at the modal layer, rgba(0,0,0,0.5) at the backdrop).

### Shadow Tokens

| Token | Value |
|---|---|
| `--shadow-card` | `0 1px 2px rgba(15,17,21,.04), 0 1px 3px rgba(15,17,21,.04)` |
| `--shadow-elevated` | `0 2px 4px rgba(15,17,21,.04), 0 8px 24px rgba(15,17,21,.08)` |
| `--shadow-modal` | `0 8px 24px rgba(15,17,21,.10), 0 24px 64px rgba(15,17,21,.16)` |
| `--shadow-focus` | `0 0 0 3px var(--color-primary-soft)` |

## Shapes

### Border Radius Scale

| Token | Value | Use |
|---|---|---|
| `{rounded.xs}` | 2px | Inline chips, tags, eyebrow badges |
| `{rounded.sm}` | 4px | Inputs, small buttons, nav items |
| `{rounded.md}` | 6px | Cards, panels |
| `{rounded.lg}` | 8px | Modals, larger cards |
| `{rounded.full}` | 9999px | Pills, avatars, toggle thumbs, status dots |

### Photography & Illustrations

The system doesn't ship photography or illustrations in product UI. The visual system relies on:

- **Charts** as the primary visual element on data-heavy pages — stacked-area for time series, donut for state breakdowns, KPI numbers for at-a-glance metrics.
- **Status dots** — small circular indicators (8px) tinted by `{colors.success}` / `{colors.danger}` / `{colors.warning}` / `{colors.primary}` for inline state signaling.
- **Mono icons** — feather / lucide-style 16px line icons, always `--color-ink-secondary` on default, `--color-primary` on active/hover. No filled icons in product UI.
- **Brand mark** — a small primary-blue geometric mark anchors the wordmark in the topbar.

## Components

### Top Navigation

**`topbar`** — 64px tall, `{colors.surface}` background in light mode, `{colors.surface-dark}` in dark, hairline bottom border. Carries the brand mark + product wordmark at left, optional breadcrumb / period-selector center, right-side cluster with theme toggle, notifications, and user avatar.

### Sidebar Navigation

**`sidebar`** — `{layout.sidebar-width}` (244px) fixed-left, `{colors.surface}` background in light, `{colors.surface-dark}` in dark. Hairline right border. Sections are `.nav-section` blocks with `.nav-section-label` eyebrows (11px `{colors.muted}` uppercase).

**`nav-link`** — 14px regular, padding 10/12, `{rounded.sm}`. Hover adds `{colors.surface-hover}` background.

**`nav-link-active`** — `{colors.primary}` text + a 3px left accent bar (`::before`) in `{colors.primary}`. The accent bar is the active-state signal — never a background tint.

**`nav-sub-link`** — the sub-navigation inside `.nav-group` (collapsible). Same accent treatment for active.

### Buttons

**`button-primary`** — The signature blue CTA. Background `{colors.primary}` (#145fe4), text `{colors.on-primary}` (white), type `{typography.button}` (14px / 600), height 36px, padding 0 16px, rounded `{rounded.sm}` (4px). Active state darkens to `{colors.primary-active}` (#0d4fc3); hover darkens to `{colors.primary-hover}` (#0e55d1). Disabled flattens to `{colors.muted}` background.

**`button-secondary`** — Surface button with hairline outline. Background `{colors.surface}`, text `{colors.ink}`, 1px `{colors.hairline}` border, same padding + height + radius as primary.

**`button-utility`** — Ghost button. Transparent background, `{colors.hairline}` border. Used for tertiary actions in a row of buttons.

**`button-danger`** — Destructive action. Background `{colors.danger}` (#d1242f), white text. Used for ban / delete / revoke operations.

### Cards & Containers

**`card`** — The default page block. 1px `{colors.hairline}` border, `{rounded.md}` (6px), `{colors.surface}` background, `--shadow-card`. Hover state shifts shadow to `--shadow-elevated`.

**`card-elevated`** — A variant without a border that relies on shadow alone for depth. Used in modals and popovers.

**`card-modal`** — The modal surface. 8px rounded, `--shadow-modal`, no border.

**`stat-card`** — A card variant for `.grid-stats`. Carries a large numeric `.stat-value` (24px semibold, `{colors.ink}`), a `.stat-label` (11px `{colors.muted}` uppercase), and optional `.stat-meta` (12px caption).

**`card-header`** — Groups an eyebrow (`.eyebrow`, 11px `{colors.primary}` uppercase), title (`<h2>`, 18px semibold), optional `.muted` paragraph, plus right-side `.card-actions`.

### Inputs & Forms

**`text-input`** — Standard text input. Background `{colors.surface}`, text `{colors.ink}`, type `{typography.body}`, `{rounded.sm}` (4px), 1px `{colors.hairline}` border, padding 8/12.

**`text-input-focused`** — Focus state. Border shifts to `{colors.primary}` + 3px `{colors.primary-soft}` outer ring (`--shadow-focus`). The soft ring is the focus signal — not a glow.

**`.form-grid`** — Two-column layout for label + input + helper. Collapses to single-column below 960px.

**`.form-row`** — Single stacked row for short forms.

### Toasts

**`toast-success`** — Fixed top-right. Background `{colors.surface}`, `--shadow-elevated`, `{rounded.md}`. Left 4px accent bar in `{colors.success}`.

**`toast-danger`** — Same as success but with `{colors.danger}` accent bar. Auto-assertive (`aria-live="assertive"`).

**`toast-info`** — Same but with `{colors.primary}` accent bar. Polite (`aria-live="polite"`).

Auto-dismisses after 4s unless `data-toast-persist`. Slides in with `--duration-base`.

### Modals

**`card-modal`** inside `.modal[hidden]` (display: none). When `.is-open`, `.modal-card` enters with translateY transition (`--duration-base`). Backdrop is rgba(0,0,0,0.5). Modals trap focus and restore it to the trigger on close.

### Tables

**`table.data`** — Full-width, hairline horizontal borders between rows, header row with `{typography.eyebrow}` muted text, hover row tint (`{colors.surface-hover}`). Numeric columns right-aligned; IP / code columns use `{typography.code}` mono.

### Tags / Badges

**`badge-eyebrow`** — Small pill label. Background `{colors.primary-soft}`, text `{colors.primary}`, `{typography.eyebrow}`, `{rounded.xs}` (2px), padding 2px 8px. Used to highlight "New" / "Beta" / status.

### Charts

**Stacked area** — 8-step blue palette (section 2.3 below). Each service uses the next palette step; "Other" overflow is `#a8ceff`. `fill-opacity: 0.78` to keep overlapping series readable. Tooltip on hover shows per-service breakdown with the same color dot. Legend dots in `.chart-legend` match polygon colors.

**Donut** — Conic gradient with the outcome palette (blue / green / amber / violet / red / teal). Used for state-mix (ban / found / unban / login success / login fail), never for service breakdown.

**Charts must read at a glance:**

- Tooltips always show totals and per-series counts.
- Legends always accompany charts.
- Axes / labels: 11px caption, muted ink. Grid lines: hairline at 25/50/75% of plot area.

## Do's and Don'ts

### Do

- Anchor every page on `{colors.canvas}` (#f6f8fb). Pure white reads as "marketing site"; the canvas tint is the working-tool differentiator.
- Reach for `{colors.primary}` (#145fe4) before any other accent. Buttons, links, focus rings, eyebrows, navigation active state — one accent, used everywhere.
- Use the 8-step blue palette for any service / intensity / magnitude chart. The blue-only story is the chart-system signature.
- Use `--space-*` tokens, not raw pixel values, in new components. The 4px base unit is the rhythm.
- Compose `{component.card}` for any grouped content surface. Hairline border + surface background + `--shadow-card` is the default.
- Pair `{typography.display}` with `{typography.body}` — same family, different size and weight. Don't introduce a second face.
- Apply `{rounded.sm}` (4px) to inputs and small buttons; `{rounded.md}` (6px) to cards; `{rounded.full}` (9999px) to pills. The radius ladder is hierarchical.
- Reserve `{colors.success}` / `{colors.danger}` / `{colors.warning}` for state. They never drive differentiation.

### Don't

- Don't add new brand colors without design approval. The system has one accent.
- Don't use `#hex` literals inside components — always go through tokens. Inline hex is implementation drift.
- Don't add drop shadows beyond `{shadow.elevated}` on cards. No neobrutalism, no glow, no multi-layer shadows.
- Don't animate beyond the three durations (`{motion.fast}` 100ms, `{motion.base}` 300ms, `{motion.slow}` 500ms) or change the easing curve (`{motion.ease}`).
- Don't mix the chart blue palette with the donut outcome palette. They're scoped — blue for intensity, multi-color for state.
- Don't bold display weight past 600. Display is semibold, never bold.
- Don't use filled icons in product UI. Line icons only, in `{colors.ink-secondary}`.
- Don't put cool grays or pure white on the canvas in light mode. `{colors.canvas}` (#f6f8fb) is the brand.

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 768px | Sidebar collapses to drawer; stat grid 1-up; `.grid-two-col` 1-up; tables horizontal scroll within card |
| Tablet | 768–1024px | Sidebar stays visible but tightens; stat grid 2-up; `.grid-settings` 1-up |
| Desktop | 1024–1440px | Full sidebar + topbar; stat grid 3-up or 4-up; `.grid-two-col` 2-up |
| Wide | > 1440px | Same as desktop; content max caps at 2560px |

### Touch Targets

- `{component.button-primary}` at minimum 36 × 16px (height × padding) — well above WCAG 44 height equivalent.
- `{component.text-input}` height is ~36px including padding; effective tap area exceeds 44px.
- `{component.nav-link}` entire row is tappable; effective tap area exceeds 44px.
- Status dots and eyebrow badges are decorative, not interactive.

### Collapsing Strategy

- Sidebar collapses to a drawer at < 768px; opens via hamburger in the topbar.
- Hero bands (display-size numbers) collapse to 24px h1 on mobile.
- Stat grids reduce columns rather than scaling cards down — `{typography.display}` (40px) becomes `{typography.h1}` (24px).
- `.grid-two-col` collapses to single column at < 960px.
- Tables retain column legibility by allowing horizontal scroll within the card rather than wrapping cells.
- Code columns in tables (IP addresses, hex codes) stay at `{typography.code}` size at every breakpoint.

### Image Behavior

- Charts scale proportionally; axis labels stay at 11px caption at every breakpoint.
- Brand mark anchors topbar at 24px on desktop, 20px on mobile.
- Status dots stay 8px at every breakpoint — they're state signals, not decorative.

## Iteration Guide

1. **Focus on ONE component at a time.** Reference its YAML key (`{component.button-primary}`, `{component.stat-card}`, `{component.card-modal}`).
2. **Variants of an existing component** (`-hover`, `-active`, `-disabled`, `-focused`) live as separate entries under `components:`. Don't combine them.
3. **Use `{token.ref}` everywhere** — never inline hex. Every color, type, radius, spacing value is referenced by token name.
4. **Document Default and Active/Pressed only.** Hover state shifts one tone; that's it. No hover state explosion.
5. **Display headlines stay at 600 / -0.01em letter-spacing.** Body stays at 400. The split is unbreakable.
6. **Brand blue (`{colors.primary}`) is the only accent.** Don't introduce a second brand color, a third chart hue, or a fourth surface tone.
7. **When in doubt about emphasis: bigger size before bigger weight.** Reach for `{typography.h1}` before bolding `{typography.body}`.
8. **Chart blue palette is monochromatic.** All 8 steps are derived from `{colors.primary}`. Don't introduce non-blue steps in service charts.
9. **Dark theme inverts only ink and surfaces.** Brand blue, semantic colors, and chart palette are unchanged.

## Known Gaps

- The system uses system fonts only. Webfont substitution (Inter, IBM Plex Sans, JetBrains Mono) is acceptable but not formalized here.
- The brand mark glyph is rendered as inline SVG; it's not formalized as a system token here. Treat it as a logo asset.
- Animation and transition easings beyond the three durations are out of scope. Page transitions, chart animations, and skeleton loaders are implementation details.
- Form validation states beyond `{component.text-input-focused}` (error / success borders) are documented narratively but not extracted as separate component entries.
- The actual product shell (sidebar + topbar + content) shares tokens with this doc but adds product-specific components (data tables with bulk actions, time-series filter chips, command palette) that are out of scope for this general design system.
- The blueprint / pipeline / API product surface carries additional components (build-step indicators, deploy-stage cards) that are out of scope here.
- Theme toggle behavior and `prefers-color-scheme` detection are not in this doc — those are runtime concerns.

---

## Appendix A — Token Quick Reference

```css
/* Brand */
--color-primary: #145fe4;
--color-primary-hover: #0e55d1;
--color-primary-active: #0d4fc3;
--color-primary-soft: rgba(20, 95, 228, 0.08);
--color-primary-soft-hover: rgba(20, 95, 228, 0.14);
--color-on-primary: #fff;

/* Surface (light) */
--color-canvas: #f6f8fb;
--color-surface: #ffffff;
--color-surface-soft: #f4f6f9;
--color-surface-hover: #eceff3;
--color-hairline: #e6e9ee;
--color-hairline-strong: #d5dae1;

/* Surface (dark) */
--color-canvas-dark: #010102;
--color-surface-dark: #0f1011;
--color-surface-dark-soft: #141516;
--color-surface-dark-hover: #18191a;
--color-hairline-dark: #23252a;
--color-primary-soft-dark: rgba(20, 95, 228, 0.15);

/* Ink */
--color-ink: #1d1d21;
--color-ink-secondary: #3f434b;
--color-muted: #67707c;
--color-ink-faint: #9aa3af;

/* Ink (dark) */
--color-ink-dark: #f7f8f8;
--color-ink-dark-secondary: #d0d6e0;
--color-muted-dark: #8a8f98;
--color-ink-faint-dark: #62666d;

/* Semantic */
--color-success: #18794e;     /* dark: #27a644 */
--color-danger: #d1242f;      /* dark: #ff6b74 */
--color-warning: #b45309;     /* dark: #e8923c */

/* Radius */
--radius-xs: 2px;
--radius-sm: 4px;
--radius-md: 6px;
--radius-lg: 8px;
--radius-full: 9999px;

/* Spacing */
--space-xxs: 4px;
--space-xs: 8px;
--space-sm: 12px;
--space-md: 16px;
--space-lg: 24px;
--space-xl: 32px;
--space-xxl: 48px;
--space-section: 64px;

/* Motion */
--ease: cubic-bezier(0.4, 0, 0.2, 1);
--duration-fast: 100ms;
--duration-base: 300ms;
--duration-slow: 500ms;

/* Layout */
--layout-sidebar-width: 244px;
--layout-topbar-height: 64px;
--layout-content-max: 2560px;
--layout-content-padding: 32px;

/* Shadow */
--shadow-card: 0 1px 2px rgba(15,17,21,.04), 0 1px 3px rgba(15,17,21,.04);
--shadow-elevated: 0 2px 4px rgba(15,17,21,.04), 0 8px 24px rgba(15,17,21,.08);
--shadow-modal: 0 8px 24px rgba(15,17,21,.10), 0 24px 64px rgba(15,17,21,.16);
--shadow-focus: 0 0 0 3px var(--color-primary-soft);
```

## Appendix B — Chart Blue Palette

```css
:root {
  /* 8-step monochromatic blue ramp, derived from #145fe4 */
  --blue-1: #0a3a8c;   /* deepest */
  --blue-2: #0d4fc3;   /* primary-active */
  --blue-3: #145fe4;   /* primary */
  --blue-4: #3b82f6;
  --blue-5: #5b9cff;
  --blue-6: #7eb6ff;
  --blue-7: #a8ceff;   /* "Other" overflow */
  --blue-8: #cfe0ff;   /* lightest */
}
```
