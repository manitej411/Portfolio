---
name: Obsidian & Ether
colors:
  surface: '#121317'
  surface-dim: '#121317'
  surface-bright: '#38393d'
  surface-container-lowest: '#0d0e12'
  surface-container-low: '#1a1b1f'
  surface-container: '#1e1f23'
  surface-container-high: '#292a2e'
  surface-container-highest: '#343539'
  on-surface: '#e3e2e7'
  on-surface-variant: '#c7c6ca'
  inverse-surface: '#e3e2e7'
  inverse-on-surface: '#2f3034'
  outline: '#919094'
  outline-variant: '#46464a'
  surface-tint: '#c8c6c7'
  primary: '#c8c6c7'
  on-primary: '#313031'
  primary-container: '#0a0a0b'
  on-primary-container: '#7a797a'
  inverse-primary: '#5f5e5f'
  secondary: '#c8c6c8'
  on-secondary: '#303032'
  secondary-container: '#474649'
  on-secondary-container: '#b7b4b7'
  tertiary: '#c8c6c8'
  on-tertiary: '#303032'
  tertiary-container: '#0a0a0c'
  on-tertiary-container: '#7a797b'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e5e2e3'
  primary-fixed-dim: '#c8c6c7'
  on-primary-fixed: '#1c1b1c'
  on-primary-fixed-variant: '#474647'
  secondary-fixed: '#e4e2e4'
  secondary-fixed-dim: '#c8c6c8'
  on-secondary-fixed: '#1b1b1d'
  on-secondary-fixed-variant: '#474649'
  tertiary-fixed: '#e4e2e4'
  tertiary-fixed-dim: '#c8c6c8'
  on-tertiary-fixed: '#1b1b1d'
  on-tertiary-fixed-variant: '#474649'
  background: '#121317'
  on-background: '#e3e2e7'
  surface-variant: '#343539'
typography:
  display:
    fontFamily: Manrope
    fontSize: 72px
    fontWeight: '200'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  h1:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '300'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  h3:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.4'
    letterSpacing: '0'
  body-lg:
    fontFamily: Noto Serif
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0.01em
  body-md:
    fontFamily: Noto Serif
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: 0.01em
  label-caps:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.15em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max-width: 1440px
  gutter: 32px
  margin-edge: 64px
  section-padding: 120px
---

## Brand & Style

This design system is built on the pillars of **Modern Minimalism** and **Glassmorphism**. It is designed for high-end creative portfolios where the content is king, but the frame is exquisite. The brand personality is "The Silent Authority"—confident, quiet, and impeccably polished. 

The aesthetic leverages deep obsidian tones to create an infinite sense of depth, utilizing translucent glass layers to organize information without breaking the visual flow. Generous whitespace (or "dark space") is used strategically to evoke a sense of luxury and breathing room, ensuring the user feels a sense of calm and focus.

## Colors

The palette is a sophisticated study in near-blacks and charcoal. The base is an absolute rich black to maximize OLED contrast, while the primary and secondary colors are used for subtle tonal layering. 

The accent is a **Soft Gold** (#D4AF37), used with extreme restraint for micro-interactions, active states, or critical calls to action. For high-end metallic feels, silver tones are achieved via low-opacity white overlays on dark backgrounds rather than a flat hex. All surface colors in this design system must support translucency to facilitate the glassmorphic effect.

## Typography

This design system utilizes a high-contrast typographic pairing to signal sophistication. **Manrope** is used for headings; its geometric but refined letterforms provide a modern, architectural feel. Headlines should use light weights (200-300) at large sizes to maintain an elegant, airy quality.

**Noto Serif** is selected for body copy to provide a literary, "fine-press" reading experience. This serif choice adds a layer of heritage and prestige to the modern interface. Labels and small navigational elements return to Manrope in uppercase with wide tracking to act as clear, functional signposts.

## Layout & Spacing

The layout philosophy follows a **Fixed Grid** with an emphasis on "The Golden Gap"—excessive vertical padding between sections to allow the eye to rest. We utilize a 12-column grid centered in the viewport.

Horizontal margins are generous (64px+) to frame the content like a piece of art in a gallery. Elements should rarely feel crowded; if in doubt, increase the spacing. Components are aligned to an 8px rhythmic grid to ensure mathematical harmony amidst the airy layout.

## Elevation & Depth

Depth is not achieved through heavy shadows but through **Glassmorphism** and light-based hierarchy. Surfaces are created using semi-transparent fills (`rgba(255, 255, 255, 0.03)`) with a high-quality background blur (20px or higher).

To define edges on dark backgrounds, use a **1px inner stroke** (rim lighting) that is slightly brighter at the top and disappears at the bottom. Shadows, when used, are "Ambient Glows"—ultra-diffused, large radius (60px+), and low opacity (10-15%) using the secondary color as the shadow tint rather than pure black.

## Shapes

The shape language is "Soft-Modern." Elements use a subtle 0.25rem (4px) corner radius to soften the technical feel of the dark mode without appearing "bubbly" or consumer-grade. Large containers or featured imagery can move to `rounded-lg` (8px) for a slightly more approachable feel. The goal is precision; corners should feel crisp but not sharp enough to be aggressive.

## Components

### Buttons
Primary buttons use a ghost style: a 1px border of the accent color or white, with a subtle background blur. Hover states involve a soft "inner glow" and a slight increase in background opacity. Typography is always `label-caps`.

### Cards & Containers
Cards must use the glassmorphic treatment. They should not have solid backgrounds. The border is a 1px solid stroke at 8% white. When stacked, the background blur of the top card should visually distort the content of the card beneath it.

### Inputs
Fields are represented by a single bottom border (1px) in a muted neutral. Upon focus, the border transitions to the soft gold accent, and a very faint vertical gradient rises from the line to suggest a focused "well."

### Chips & Tags
Small, pill-shaped elements with a high-transparency background (`rgba(255, 255, 255, 0.05)`) and `label-caps` text. They serve as metadata markers without distracting from the primary imagery.

### Additional Components: Image Lightbox
Since this is a portfolio system, the lightbox is critical. It should utilize a 95% opacity black backdrop with zero blur, making the artwork the sole focus of the interface.