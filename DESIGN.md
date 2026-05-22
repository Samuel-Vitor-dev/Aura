---
name: Quiet Luxury Interior Design System
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#38393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#c4c7c7'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c8c6c5'
  primary: '#c8c6c5'
  on-primary: '#313030'
  primary-container: '#121212'
  on-primary-container: '#7e7d7d'
  inverse-primary: '#5f5e5e'
  secondary: '#e9c349'
  on-secondary: '#3c2f00'
  secondary-container: '#af8d11'
  on-secondary-container: '#342800'
  tertiary: '#e9c176'
  on-tertiary: '#412d00'
  tertiary-container: '#1a1000'
  on-tertiary-container: '#997835'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5e2e1'
  primary-fixed-dim: '#c8c6c5'
  on-primary-fixed: '#1c1b1b'
  on-primary-fixed-variant: '#474646'
  secondary-fixed: '#ffe088'
  secondary-fixed-dim: '#e9c349'
  on-secondary-fixed: '#241a00'
  on-secondary-fixed-variant: '#574500'
  tertiary-fixed: '#ffdea5'
  tertiary-fixed-dim: '#e9c176'
  on-tertiary-fixed: '#261900'
  on-tertiary-fixed-variant: '#5d4201'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  display-lg:
    fontFamily: Bodoni Moda
    fontSize: 64px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Bodoni Moda
    fontSize: 40px
    fontWeight: '400'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Bodoni Moda
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '300'
    lineHeight: '1.6'
    letterSpacing: 0.01em
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.2em
spacing:
  unit: 8px
  container-max: 1440px
  gutter: 24px
  margin-desktop: 80px
  margin-mobile: 24px
  section-gap: 160px
---

## Brand & Style

This design system is anchored in the concept of "Quiet Luxury," emphasizing architectural precision, material honesty, and the curated atmosphere of a private gallery. The target audience is high-net-worth individuals who value discretion, timeless elegance, and meticulous craftsmanship.

The style is defined by **Minimalism** blended with **Tactile** refinement. It avoids superficial ornamentation in favor of structural integrity. The interface must feel like an editorial publication—spacious, authoritative, and serene. Every interaction should evoke the hushed, deliberate pace of a boutique hotel lobby or a high-end art exhibition.

## Colors

The palette is intentionally restricted to evoke exclusivity and depth. 
- **Base Layers:** The foundation uses `background_deep` (#0A0A0A) for total immersion. Secondary surfaces utilize `surface_charcoal` to create subtle structural differentiation without losing the monochromatic weight.
- **Accents:** The "Champagne Gold" (`accent_gold_champagne`) is used sparingly—only for high-priority calls to action, active states, or delicate architectural lines. It should never dominate the screen.
- **Typography:** Primary information uses pure white for maximum legibility against the dark void, while `text_secondary` (a soft, muted grey) handles metadata and supporting descriptions to maintain visual hierarchy.

## Typography

The typographic system relies on the dramatic contrast between the high-stroke variance of **Bodoni Moda** and the clinical precision of **Hanken Grotesk**.

- **Headlines:** Use Bodoni Moda for all main titles. It functions as a visual texture. Large display sizes should use negative letter spacing to emphasize the editorial look.
- **Body Text:** Hanken Grotesk provides a modern, neutral counterpoint. A lighter weight (300) is preferred for long-form text to keep the interface feeling "airy" despite the dark theme.
- **Labels:** Small labels and navigational elements should be set in uppercase with generous letter spacing to evoke the branding found on luxury product packaging.

## Layout & Spacing

The layout follows a **fixed grid** philosophy for desktop to maintain rigorous alignment, transitioning to a fluid model for mobile. 

- **Negative Space:** Immense vertical gaps (`section-gap`) are required between content blocks to allow the "art" (images) to breathe. The design system prioritizes a "less is more" approach; do not crowd the viewport.
- **Alignment:** Use a 12-column grid. Elements should often be offset—for example, a headline spanning columns 2-6 while the body text starts at column 7—to mimic gallery wall layouts.
- **Margins:** Desktop margins are intentionally wide (80px+) to frame the content, acting like a passe-partout in a picture frame.

## Elevation & Depth

Hierarchy is established through **Tonal Layers** and **Ambient Shadows** rather than traditional elevation.

- **Surfaces:** Depth is achieved by placing `surface_charcoal` elements over the `background_deep` floor. 
- **Shadows:** Use ultra-diffused shadows (e.g., `0 20px 50px rgba(0,0,0,0.5)`). Shadows should feel like ambient occlusion in a dimly lit room, adding weight and presence to cards and floating navigation bars.
- **Interactions:** Use subtle backdrop blurs (Glassmorphism) on sticky navigation elements to provide a sense of transparency and lightness, allowing the high-resolution interior photography to bleed through slightly as the user scrolls.

## Shapes

The shape language is strictly **Sharp (0)**. 

Every element—buttons, input fields, image containers, and cards—must feature 90-degree angles. This reinforces the architectural nature of the brand and the "nítida" (crisp) visual style. Roundness is perceived as too soft or consumer-grade for this high-end context. Dividers should be hair-line thin (0.5px to 1px) using the gold or dark grey palette.

## Components

- **Buttons:** Primary buttons are outlined in `accent_gold_champagne` with no fill, or solid black with a thin gold border. Text is always `label-caps`. Hover states should involve a slow, elegant color fill or a slight expansion of the letter spacing.
- **Cards:** Cards should have no visible borders by default. They rely on the `surface_charcoal` background and deep ambient shadows to separate themselves from the floor.
- **Input Fields:** Minimalist under-line inputs only. No bounding boxes. The label sits above in `label-caps`.
- **Navigation:** A persistent but discrete top bar. Use high-contrast transitions (e.g., a gold line appearing beneath an active link) with a duration of 400ms to ensure "elegance."
- **Imagery:** All images must be treated as hero elements. Use subtle zoom-in transitions on scroll or hover to simulate a cinematic experience.
- **Custom Components:** Include "Project Spotlights"—large-scale image carousels with minimal overlaid Bodoni Moda typography and "Floor Plan Viewers" using thin gold vector lines.