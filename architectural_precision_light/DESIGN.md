---
name: Architectural Precision Light
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#454556'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#767588'
  outline-variant: '#c6c4d9'
  surface-tint: '#3e3ef8'
  primary: '#2924e8'
  on-primary: '#ffffff'
  primary-container: '#4748ff'
  on-primary-container: '#e3e2ff'
  inverse-primary: '#c0c1ff'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#8d2d00'
  on-tertiary: '#ffffff'
  tertiary-container: '#b63c00'
  on-tertiary-container: '#ffddd2'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e1e0ff'
  primary-fixed-dim: '#c0c1ff'
  on-primary-fixed: '#06006c'
  on-primary-fixed-variant: '#1f13e2'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#ffdbcf'
  tertiary-fixed-dim: '#ffb59b'
  on-tertiary-fixed: '#380d00'
  on-tertiary-fixed-variant: '#812800'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  headline-xl:
    fontFamily: Metrophobic
    fontSize: 48px
    fontWeight: '400'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Metrophobic
    fontSize: 32px
    fontWeight: '400'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Metrophobic
    fontSize: 28px
    fontWeight: '400'
    lineHeight: 36px
  headline-md:
    fontFamily: Metrophobic
    fontSize: 24px
    fontWeight: '400'
    lineHeight: 32px
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '500'
    lineHeight: 14px
    letterSpacing: 0.08em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: '4'
  gutter: '24'
  margin-desktop: '64'
  margin-mobile: '16'
  container-max: '1440'
---

## Brand & Style
This design system embodies the clarity, structure, and intent of modern architectural drafting. It targets professional environments where precision and information density are paramount—specifically technical SaaS, architecture firms, and high-end engineering tools.

The aesthetic is a refined blend of **Minimalism** and **Corporate Modernism**. It prioritizes extreme legibility, disciplined whitespace, and a rhythmic use of grids. The transition to light mode emphasizes a "gallery" feel: clean white expanses, subtle structural dividers, and a singular, vibrant electric indigo accent that directs focus without overwhelming the senses. The emotional response is one of organized calm, reliability, and high-functioning utility.

## Colors
The palette is anchored by the Electric Indigo accent, used sparingly for primary actions and critical status indicators. 

- **Primary:** Electric Indigo (#4748ff) serves as the "active" signal.
- **Background:** Pure White (#ffffff) provides the highest possible contrast for text.
- **Surfaces:** Light Slate-Grey (#f8fafc) is used for container backgrounds and sidebars to create subtle structural differentiation.
- **Text:** Deep Charcoal (#0f172a) is used for headlines and primary body copy to ensure AA/AAA accessibility. 
- **Subtext:** Mid-Slate (#64748b) is reserved for secondary information and captions.
- **Borders:** A consistent light grey (#e2e8f0) defines the architectural boundaries of the UI.

## Typography
The typography strategy reinforces the technical nature of the design system. **Metrophobic** provides a structured, geometric feel for headlines. **Hanken Grotesk** is used for body copy due to its exceptional clarity and modern proportions. **JetBrains Mono** is utilized for labels, metadata, and technical data points, evoking the precision of code and blueprints.

Large headlines should use slight negative letter-spacing to maintain a "tight" architectural feel. Labels should always be uppercase when used for section headers or small metadata to distinguish them from flow text.

## Layout & Spacing
The layout follows a **Fixed Grid** philosophy on desktop and a **Fluid Grid** on mobile. The system is built on a 4px baseline shift, ensuring all components and spacing increments are multiples of 4.

- **Desktop (1440px+):** 12-column grid with 24px gutters and 64px outer margins.
- **Tablet (768px - 1439px):** 8-column grid with 20px gutters and 32px outer margins.
- **Mobile (Under 768px):** 4-column grid with 16px gutters and 16px outer margins.

Spacing should be generous to allow the "structural" elements (borders and lines) to breathe. Content is grouped using padding rather than heavy background fills.

## Elevation & Depth
In this design system, depth is communicated through **Tonal Layers** and **Low-Contrast Outlines** rather than traditional shadows. 

- **Level 0 (Background):** Pure white (#ffffff).
- **Level 1 (Containers/Sidebars):** Light Slate (#f8fafc) with a 1px border (#e2e8f0).
- **Level 2 (Modals/Popovers):** Pure white with a very fine, highly diffused ambient shadow (0px 4px 20px rgba(15, 23, 42, 0.05)) to suggest a gentle lift off the page.
- **Separators:** Use 1px solid lines (#f1f5f9) to divide content within a single container. 

Avoid heavy dropshadows or blurring effects; the goal is a flat, "blueprint-style" stack of papers.

## Shapes
Shapes are disciplined and "Soft" (0.25rem). This slight rounding prevents the UI from feeling aggressive or overly Brutalist while maintaining the precision of a technical tool. 

- **Small elements (Checkboxes, Tags):** 2px radius.
- **Standard elements (Buttons, Inputs, Cards):** 4px radius (0.25rem).
- **Large elements (Modals, Large Containers):** 8px radius (0.5rem).

Interactive elements should never be pill-shaped; they must maintain a rectangular structure to align with the grid-heavy aesthetic.

## Components

- **Buttons:** Primary buttons use a solid Indigo (#4748ff) fill with white text. Secondary buttons use a white background with a 1px border (#e2e8f0) and Charcoal text. Use a 4px radius.
- **Inputs:** Text fields use a 1px border (#e2e8f0). On focus, the border changes to Indigo (#4748ff) with a subtle 2px outer glow of the same color at 10% opacity.
- **Chips/Tags:** Use the JetBrains Mono label-sm font. Background should be a very light tint of the neutral color (#f1f5f9) with Charcoal text.
- **Lists:** Use subtle 1px horizontal dividers (#f1f5f9). Hover states on list items should utilize a change to the surface color (#f8fafc) rather than a shadow.
- **Checkboxes & Radios:** Use the Indigo color for the "Checked" state. Maintain the 2px radius for checkboxes for a consistent "Soft" shape language.
- **Cards:** Cards should be white with a 1px border (#e2e8f0). No shadows unless the card is interactive/hoverable, in which case it may lift slightly with a faint ambient shadow.
- **Data Tables:** High-density layout with 12px vertical padding. Headers use JetBrains Mono in uppercase with a light grey background (#f8fafc).