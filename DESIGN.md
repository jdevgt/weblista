---
name: Neo-Brutalist Launchpad
colors:
  surface: '#FFFFFF'
  surface-dim: '#d4dbdd'
  surface-bright: '#f3fbfc'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#edf5f7'
  surface-container: '#e8eff1'
  surface-container-high: '#e2e9eb'
  surface-container-highest: '#dce4e5'
  on-surface: '#151d1e'
  on-surface-variant: '#3b494c'
  inverse-surface: '#2a3233'
  inverse-on-surface: '#eaf2f4'
  outline: '#6b7a7d'
  outline-variant: '#bac9cc'
  surface-tint: '#006875'
  primary: '#006875'
  on-primary: '#ffffff'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#00daf3'
  secondary: '#506600'
  on-secondary: '#ffffff'
  secondary-container: '#c1f100'
  on-secondary-container: '#546b00'
  tertiary: '#5e5e5e'
  on-tertiary: '#ffffff'
  tertiary-container: '#d0d0d0'
  on-tertiary-container: '#595959'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#c3f400'
  secondary-fixed-dim: '#abd600'
  on-secondary-fixed: '#161e00'
  on-secondary-fixed-variant: '#3c4d00'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#f3fbfc'
  on-background: '#151d1e'
  surface-variant: '#dce4e5'
  border-black: '#000000'
  error-red: '#EF4444'
  success-green: '#25D366'
typography:
  display-xl:
    fontFamily: Archivo Black
    fontSize: 88px
    fontWeight: '900'
    lineHeight: '0.9'
    letterSpacing: -0.05em
  display-xl-mobile:
    fontFamily: Archivo Black
    fontSize: 56px
    fontWeight: '900'
    lineHeight: '0.9'
    letterSpacing: -0.05em
  headline-lg:
    fontFamily: Archivo Black
    fontSize: 64px
    fontWeight: '900'
    lineHeight: '1.0'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Archivo Black
    fontSize: 40px
    fontWeight: '900'
    lineHeight: '1.1'
  title-lg:
    fontFamily: Archivo Black
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.1'
  body-xl:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  body-md:
    fontFamily: Space Grotesk
    fontSize: 18px
    fontWeight: '700'
    lineHeight: '1.3'
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '700'
    lineHeight: '1.0'
  nav-link:
    fontFamily: Archivo Black
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.0'
    letterSpacing: 0.05em
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  xxl: 80px
  container-max: 1000px
  gutter: 24px
---

## Brand & Style

This design system is rooted in **Neo-Brutalism**. It is designed for businesses that want to appear disruptive, high-energy, and transparent. The brand personality is "Industrial-Chic": raw, confident, and unapologetically functional. 

The aesthetic is characterized by heavy black outlines, stark shadows, and a "physical" depth that mimics paper layers or industrial signage. It avoids gradients and soft blurs in favor of flat color blocks and sharp geometric shapes. The target audience is modern entrepreneurs and digital-native businesses looking for a "done-for-you" service that feels as robust as it is fast.

## Colors

The palette uses high-contrast "Electric" tones against a strictly monochrome foundation. 

- **Primary (#00E5FF):** Used for primary actions, highlight blocks, and "Key" solution elements. It signifies innovation and digital speed.
- **Secondary (#CCFF00):** An acidic lime used for phase indicators, accents, and "Popular" tags. It draws the eye to specific points of interest.
- **Tertiary/Ink (#000000):** The structural backbone. Every border, shadow, and heavy text element uses pure black.
- **Surface (#FFFFFF):** The canvas. Used to provide maximum contrast for the heavy borders and vibrant accents.

Interaction states do not use subtle fades; instead, they use "Offset Hover" effects (translating the element to cover its own shadow).

## Typography

The typography strategy is "Aggressive Legibility." 

- **Display & Headlines:** Uses **Archivo Black**. It must always be uppercase with tight tracking. On desktop, large display text should utilize a 0.9 line-height to create a dense, impactful "wall of text" effect.
- **Body:** Uses **Space Grotesk** at a heavy weight (Bold/700). In Neo-Brutalism, "regular" weights often feel too weak; bold body text maintains the visual weight of the heavy borders.
- **Technical Info:** Uses **JetBrains Mono** for secondary details, payment trust markers, or small captions to evoke a "system-generated" feel.

## Layout & Spacing

The system uses a **Fixed Grid** model for desktop, centered with a max-width of 1000px to maintain readability and vertical rhythm. 

- **Section Spacing:** Use `xxl` (80px) for vertical padding between major sections.
- **Component Spacing:** Utilize `lg` (24px) for gaps between cards or grid items.
- **The "Tilt" Rule:** To break the rigidity of the grid, secondary accents (chips, badges, or small cards) should be rotated between -2 and 2 degrees. This adds to the "hand-pasted" look of the design.
- **Mobile:** Breakpoints at 768px. On mobile, horizontal padding should stay at `gutter` (24px) and multi-column grids should collapse to 1-column stacks.

## Elevation & Depth

Depth is achieved through **Hard Shadows** rather than Z-axis blurs. 

- **Brutal Shadow:** Every interactive element (buttons, cards, input fields) features a solid 8px black shadow at a 45-degree angle (bottom-right). For larger cards, this can increase to 16px.
- **Shadow Inversion:** On dark backgrounds, the shadow color switches from Black to White (#FFFFFF).
- **Interaction Logic:** Buttons do not "grow" on hover. Instead, they use a `translate-x-[4px] translate-y-[4px]` transform that moves the element into its own shadow area, effectively "pressing" the element into the page.

## Shapes

The shape language is **Strictly Geometric and Sharp**.

- **Corners:** 0px radius for all structural elements (cards, buttons, banners). 
- **Exceptions:** Circular elements (radius: 9999px) are permitted only for specific functional icons, step numbers, or user avatars to create a "badge" or "stamp" effect.
- **Borders:** A consistent 4px solid black border must be applied to all primary containers.

## Components

- **Buttons:** 4px black border, solid color background (Primary or White), uppercase Archivo Black text. Must include a brutal shadow.
- **Cards:** White background, 4px black border, 8px shadow. Include an optional 1-2 degree rotation for secondary cards.
- **Accordions (FAQ):** Sharp borders between items. Active items should change background color to the Primary color (#00E5FF) and show a top border on the content area.
- **Badges/Chips:** Small rectangular boxes with secondary colors (#CCFF00), 4px borders, and tilted rotation.
- **Input Fields:** 4px black border, no roundedness, bold Space Grotesk text. Focused states should not use glow, but rather a color shift in the border or a background tint.
- **Icons:** Use **Material Symbols Outlined** with a consistent stroke weight (usually bold/700) to match the typography's visual weight.