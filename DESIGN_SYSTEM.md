# Portfolio Design System

A comprehensive design system extracted from the Paul T Hanson portfolio website, built with modern web standards for responsive, accessible experiences.

## Overview

This design system provides a complete set of design tokens, components, and patterns used throughout the portfolio website. It's designed to be:

- **Minimal & focused** - Clean, essential components for a portfolio
- **Responsive** - Mobile-first approach with fluid typography
- **Accessible** - High contrast, semantic HTML, readable line-height
- **Maintainable** - Clear naming conventions and documented patterns

---

## Color Palette

### Primary Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Primary Blue | `#2563eb` | Buttons, links, accents |
| Primary Dark | `#1d4ed8` | Hover states, active states |

### Text Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Primary | `#0f172a` | Headings, primary text |
| Secondary | `#475569` | Body copy |
| Tertiary | `#334155` | Navigation, secondary links |
| Subtle | `#64748b` | Footer, captions, metadata |

### Background Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Page | `#f8fafc` | Main background |
| Card | `#ffffff` | Card surfaces |
| Alt | `#f8fafc` | Alternative surfaces |

### Border Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Light | `#e2e8f0` | Subtle dividers |
| Medium | `#cbd5e1` | Standard borders |

### Accent Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Lime Green | `#84cc16` | Highlights, emphasis (favorite) |

---

## Typography

### Font Family

```
Inter, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif
```

**Features:** `cv02`, `cv04` (OpenType feature settings for visual refinement)

### Type Scale

#### Display Large
- **Size:** `clamp(2rem, 4vw, 3.5rem)` (responsive)
- **Weight:** 700 (Bold)
- **Line Height:** 1.1
- **Letter Spacing:** -0.05em
- **Usage:** Hero titles, page headers

#### Display Medium
- **Size:** `clamp(2rem, 5vw, 3.25rem)` (responsive)
- **Weight:** 700 (Bold)
- **Line Height:** 1.05
- **Usage:** Hero section headings

#### Heading XL
- **Size:** 1.5rem (24px)
- **Weight:** 700 (Bold)
- **Usage:** Section titles

#### Heading Large
- **Size:** 1.1rem (17.6px)
- **Weight:** 700 (Bold)
- **Usage:** Card titles, subheadings

#### Body
- **Size:** 1rem (16px)
- **Weight:** 400 (Regular)
- **Line Height:** 1.6
- **Usage:** Primary body text, paragraphs

#### Body Small
- **Size:** 0.875rem (14px)
- **Weight:** 400
- **Usage:** Secondary text, descriptions

#### Label / Eyebrow
- **Size:** 0.8rem (12.8px)
- **Weight:** 600 (Semibold)
- **Text Transform:** uppercase
- **Letter Spacing:** 0.24em - 0.28em
- **Usage:** Accents, labels, section markers

---

## Spacing

### Spacing Scale

Consistent spacing maintains visual harmony across all components.

| Token | Size | Usage |
|-------|------|-------|
| `xs` | 0.5rem (8px) | Tight spacing |
| `sm` | 0.75rem (12px) | Small gaps |
| `md` | 1rem (16px) | Base spacing unit |
| `lg` | 1.5rem (24px) | Medium gaps |
| `xl` | 2rem (32px) | Large gaps |
| `2xl` | 2.5rem (40px) | Extra large spacing |

### Layout Tokens

- **Max Width:** 1100px
- **Horizontal Gutter:** 2rem (32px)
- **Card Padding:** 1.75rem (28px)
- **Default Gap:** 1rem (16px)
- **Line Height:** 1.6 (for readability)

---

## Border Radius

| Token | Size | Usage |
|-------|------|-------|
| Small | 1rem (16px) | Small cards, buttons |
| Medium | 1.25rem (20px) | Standard cards |
| Large | 1.5rem (24px) | Hero sections |
| Full | 999px | Pills, rounded buttons |

---

## Shadows

### Elevation Levels

#### Section Shadow (Light)
```css
box-shadow: 0 20px 40px rgba(15, 23, 42, 0.06);
```
- Used on section cards and standard surfaces
- Subtle, minimal elevation

#### Hero Shadow (Medium)
```css
box-shadow: 0 30px 60px rgba(15, 23, 42, 0.08);
```
- Used on hero sections and featured content
- More pronounced elevation for prominence

---

## Components

### Button

**States & Variants**

- **Primary Button**
  - Background: `#2563eb`
  - Padding: `0.95rem 1.6rem`
  - Border Radius: `999px`
  - Font Weight: 700
  - Hover: Background darkens to `#1d4ed8`, slight vertical shift

- **Outline Button**
  - Background: Transparent
  - Border: `2px solid #2563eb`
  - Color: `#2563eb`
  - Same padding and border radius as primary

**Interaction:**
- Transition: `transform 0.2s ease, background 0.2s ease`
- Hover Effect: `transform: translateY(-1px)` (lift effect)

### Card

**Section Card**
- Padding: `1.75rem`
- Background: `#ffffff`
- Border Radius: `1.25rem`
- Shadow: Section shadow (light)
- Margin Bottom: `1.5rem`

**Project Card**
- Padding: `1.5rem`
- Background: `#f8fafc`
- Border: `1px solid #e2e8f0`
- Border Radius: `1rem`
- Lightweight alternative to full shadow cards

### Skill Pill

- Padding: `0.9rem 1rem`
- Border Radius: `999px`
- Border: `1px solid #cbd5e1`
- Background: `#ffffff`
- Font Weight: 600
- Text Align: center

### Grid Layouts

**Skill Grid**
- Columns: `repeat(auto-fit, minmax(160px, 1fr))`
- Gap: `0.75rem`

**Project Grid**
- Columns: `repeat(auto-fit, minmax(240px, 1fr))`
- Gap: `1rem`

---

## Responsive Breakpoints

### Mobile First Approach

**Small Screen (< 640px)**
- Adjusted padding and margins
- Centered navigation and footer
- Stack layout for better mobile experience

**Medium & Large Screens (≥ 640px)**
- Full layout with horizontal navigation
- Multi-column grids
- Fluid typography scales up

---

## Usage Examples

### Creating a New Section Card

```html
<section class="section-card">
  <h3>Section Title</h3>
  <p>Your content here...</p>
</section>
```

### Button Variations

```html
<!-- Primary -->
<a class="button" href="#target">Primary Action</a>

<!-- Outline -->
<a class="button button-outline" href="#target">Secondary Action</a>
```

### Skill Pill Grid

```html
<div class="skill-grid">
  <div class="skill-pill">Your Skill</div>
  <div class="skill-pill">Another Skill</div>
</div>
```

---

## Design Principles

1. **Hierarchy** - Clear visual priority through size, weight, and color
2. **Whitespace** - Generous spacing for breathing room and focus
3. **Consistency** - Repeating patterns create predictability
4. **Accessibility** - High contrast, readable fonts, semantic HTML
5. **Performance** - Minimal, optimized CSS with no unnecessary effects

---

## Files

- **`src/design-tokens.json`** - Structured design token definitions
- **`src/style.css`** - Main stylesheet with all components
- **`DESIGN_SYSTEM.md`** - This documentation
- **Design System Canvas** - Interactive visual reference (Artifact)

---

## Extending the Design System

When adding new colors or components:

1. Define the token in `design-tokens.json`
2. Add corresponding CSS to `src/style.css`
3. Document the component with usage examples
4. Update the visual reference in the Design System canvas

---

*Last Updated: 2026-09-17*
