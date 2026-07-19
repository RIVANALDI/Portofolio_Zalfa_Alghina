---
name: Architectural Precision
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#cdc3d6'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#968d9f'
  outline-variant: '#4b4454'
  surface-tint: '#9ccaff'
  primary: '#9ccaff'
  on-primary: '#003256'
  primary-container: '#004b7d'
  on-primary-container: '#7bbcff'
  inverse-primary: '#0062a1'
  secondary: '#f3aeff'
  on-secondary: '#55006b'
  secondary-container: '#9301b6'
  on-secondary-container: '#f5b8ff'
  tertiary: '#ffb4a8'
  on-tertiary: '#690000'
  tertiary-container: '#8f170e'
  on-tertiary-container: '#ff9d8e'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#d0e4ff'
  primary-fixed-dim: '#9ccaff'
  on-primary-fixed: '#001d35'
  on-primary-fixed-variant: '#00497a'
  secondary-fixed: '#fcd6ff'
  secondary-fixed-dim: '#f3aeff'
  on-secondary-fixed: '#340042'
  on-secondary-fixed-variant: '#790096'
  tertiary-fixed: '#ffdad4'
  tertiary-fixed-dim: '#ffb4a8'
  on-tertiary-fixed: '#410000'
  on-tertiary-fixed-variant: '#8d160c'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: Hanken Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.5'
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  section-gap: 120px
---

## Brand & Style
The brand personality is authoritative yet approachable, reflecting a high-end professional identity. The target audience includes creative directors, hiring managers, and high-value clients who prioritize clarity and technical excellence.

The design system employs a **Modern Minimalist** style with a focus on high-quality typography and structured whitespace. It borrows elements from **Corporate Modern** design—utilizing a rigorous grid—while incorporating subtle **Glassmorphism** for navigational elements to maintain a sense of lightness and depth. The goal is to evoke a sense of calm, precision, and meticulous craft.

## Colors
This design system utilizes a sophisticated "Triadic Depth" palette. The primary accent is a professional **Deep Azure Blue**, providing a stable and technical foundation for calls to action and core branding elements.

In **Dark Mode** (default), the background uses deep, neutral tones to reduce eye strain and provide a premium canvas for portfolio imagery. Neutral tones are derived from a **Deep Onyx** (#0c0c0c), shifting the interface toward a profound, ink-like black. 

The palette is enriched by two supporting accents:
- **Secondary:** A **Deep Magenta** provides high-energy pops against the dark canvas.
- **Tertiary:** A **Deep Garnet** (#750000) adds a layer of serious, low-light emphasis for specialized states or critical information, ensuring the system remains anchored and professional.

## Typography
The typography strategy pairs a technical, sharp sans-serif for impact with a highly legible utilitarian face for content.

- **Headlines:** Use **Hanken Grotesk** for its clean, contemporary feel. Large display sizes should use tight letter-spacing to emphasize the "architectural" structure of the letterforms.
- **Body:** **Inter** provides exceptional readability across all screen sizes and themes.
- **Labels/Technical Data:** **JetBrains Mono** is used for dates, tags, and small captions to inject a hint of "developer-ready" precision.

## Layout & Spacing
This design system follows a **12-column fixed grid** for desktop and a **4-column fluid grid** for mobile. 

- **Vertical Rhythm:** Built on an 8px baseline. Use `section-gap` for major layout transitions to ensure the "Minimalist" aesthetic is maintained through ample whitespace.
- **Responsiveness:** On mobile, margins shrink to 16px, and section gaps are reduced to 64px. Content should reflow into a single column, with cards expanding to full width.

## Elevation & Depth
Hierarchy is established through **Tonal Layers** rather than heavy shadows. 

- **Level 0 (Surface):** The main background (`bg-primary`).
- **Level 1 (Cards/Floating):** Use container surfaces with a subtle 1px border. 
- **Navigation:** Employs a **Glassmorphism** effect with a `12px` backdrop blur and 80% opacity of the surface color to keep the user oriented within the long-scroll portfolio context.
- **Shadows:** Only used on active states or primary buttons—very soft, tinted with the primary accent color (e.g., `rgba(5, 103, 168, 0.2)`).

## Shapes
The design system uses a **Soft** shape language. This ensures the professional "sturdiness" of the UI remains intact without feeling clinical. 

- **Small elements (Buttons, Inputs):** 0.25rem (4px).
- **Medium elements (Cards, Modals):** 0.75rem (12px).
- **Full-bleed images:** Should remain sharp (0px) to contrast with the UI components.

## Components

### Theme Toggle
A critical component located in the top-right navigation. In Dark Mode, the icon should be a soft azure-white; in Light Mode, a deep onyx gray.

### Buttons
- **Primary:** Solid background (Deep Azure), white text, sharp corners with subtle rounding (4px).
- **Secondary:** Ghost style (border only), transitioning to a subtle background fill on hover using the Deep Magenta accent.
- **Tertiary/Status:** Subtle accents or outlines using the Deep Garnet color for specific semantic meaning.

### Portfolio Cards
Feature a "contained" style. Large imagery on top, with a metadata footer using `label-sm` (JetBrains Mono) for tags. The card background should be a surface container to distinguish it from the main Deep Onyx canvas.

### Navigation
A fixed header with a backdrop blur. Links use `label-sm` for a technical, organized look. The "active" link is indicated by a 2px bottom border in the Deep Azure accent color.

### Inputs
Minimalist underlines or very subtle 1px borders. Focus states should clearly highlight the entire input field with a glow using the Deep Azure accent color.