---
name: Aureate Heritage
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#4d463b'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#7f7669'
  outline-variant: '#d0c5b6'
  surface-tint: '#735b2e'
  primary: '#735b2e'
  on-primary: '#ffffff'
  primary-container: '#cdae7a'
  on-primary-container: '#574117'
  inverse-primary: '#e2c28c'
  secondary: '#5f5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e2dfde'
  on-secondary-container: '#636262'
  tertiary: '#5d5f5f'
  on-tertiary: '#ffffff'
  tertiary-container: '#b1b2b2'
  on-tertiary-container: '#434545'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdea8'
  primary-fixed-dim: '#e2c28c'
  on-primary-fixed: '#271900'
  on-primary-fixed-variant: '#594319'
  secondary-fixed: '#e5e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1c1b1b'
  on-secondary-fixed-variant: '#474746'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c7'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  display-lg:
    fontFamily: Libre Caslon Text
    fontSize: 64px
    fontWeight: '400'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Libre Caslon Text
    fontSize: 40px
    fontWeight: '400'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Libre Caslon Text
    fontSize: 32px
    fontWeight: '400'
    lineHeight: '1.3'
  headline-sm:
    fontFamily: Libre Caslon Text
    fontSize: 24px
    fontWeight: '400'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.1em
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 20px
  margin-desktop: 64px
  section-gap: 120px
---

## Brand & Style

The design system is rooted in the "New Minimalist" aesthetic—a blend of high-end editorial layouts and warm, tactile sophistication. It is designed to evoke the sensory experience of a premium boutique café: the aroma of artisanal coffee, the texture of heavy cardstock menus, and the quiet luxury of a sun-drenched interior.

The target audience consists of discerning enthusiasts who value craft and intentionality. To achieve this, the UI utilizes generous whitespace (the "luxury of breath"), precise typographic hierarchy, and subtle transitions. The interface remains quiet, allowing cinematic video content and high-fidelity photography to provide the emotional core, while the functional elements act as elegant, gold-trimmed frames for the experience.

## Colors

The palette is restrained and intentional, mimicking the natural materials found in high-end architecture.

*   **Primary (Warm Gold):** Used sparingly for interactive accents, active states, and signature branding elements. It should feel like a metallic inlay rather than a loud highlight.
*   **Neutral (Off-white):** The #F5F5F5 base provides a softer, more sophisticated foundation than pure white, reducing eye strain and feeling more "organic."
*   **Secondary (Charcoal/Ink):** Used for primary text to ensure high legibility while maintaining a softer contrast than true black.
*   **Surface (White):** Reserved for elevated cards or floating elements to create a subtle sense of depth against the off-white background.

## Typography

This design system employs a classic serif/sans-serif pairing to balance heritage with modernity. 

**Libre Caslon Text** is used for all headlines and display moments. Its literary roots provide an authoritative yet graceful presence. For large display sizes, use slight negative letter-spacing to create a tighter, editorial feel.

**Hanken Grotesk** serves as the functional workhorse. It is a clean, contemporary sans-serif that remains legible at small sizes. Use the "Label Caps" style for navigation links, category tags, and small buttons to introduce a structured, rhythmic contrast to the fluid serif headlines.

## Layout & Spacing

The layout philosophy is built on "The Gallery Grid"—a 12-column fixed grid that prioritizes vast margins to focus the user's eye on specific focal points. 

*   **Sectional Rhythm:** Use a generous 120px vertical gap between major content blocks to prevent the interface from feeling cluttered.
*   **Hero Overlay:** The navigation and hero elements must use a `backdrop-filter: blur(10px)` or a subtle gradient overlay (from 40% black to transparent) when positioned over the video background to ensure WCAG-compliant contrast for the gold and white text.
*   **Asymmetry:** Occasionally break the grid with images that span 7 or 8 columns, leaving the remaining space empty to enhance the minimalist aesthetic.

## Elevation & Depth

This design system avoids heavy drop shadows in favor of **Tonal Layering** and **Micro-Borders**.

Depth is communicated through:
1.  **Planes:** A pure white (`#FFFFFF`) surface elevated slightly above the off-white (`#F5F5F5`) background.
2.  **Stroke:** Elements like cards or input fields use a 1px solid border in a slightly darker neutral tone (5% opacity black) rather than a shadow.
3.  **Glass:** For the navigation bar and video overlays, use a semi-transparent white (80% opacity) with a high-saturation backdrop blur to create a "frosted gold" effect when it interacts with the video content.

## Shapes

The shape language is strictly **Sharp (0)**. 

To maintain a sophisticated, high-fashion architectural feel, this design system rejects rounded corners. All buttons, image containers, cards, and input fields must have crisp 90-degree angles. This severity is balanced by the softness of the color palette and the organic nature of the serif typography.

## Components

*   **Buttons:** Primary buttons feature a solid Gold background with White text. Secondary buttons are "Ghost" style: a 1px Gold border with Gold text. On hover, the primary button should shift slightly in hue or darken by 5%, while the ghost button should fill with a very pale gold tint (10% opacity).
*   **Navigation:** A minimal top bar. Links use the `label-caps` style. The "Book a Table" or "Order Now" action is a Ghost button. On scroll, the bar transitions from transparent to the frosted glass effect.
*   **Input Fields:** Single-line bottom borders only. The label sits above in `label-caps`. When focused, the bottom border transitions from a light gray to the Primary Gold.
*   **Cards:** Rectangular containers with no shadow. Use a 1px subtle border. Images within cards should have a "zoom" effect on hover to add a layer of interactivity without moving layout elements.
*   **Menu Lists:** Clean typography-first lists. The item name is in a semi-bold sans-serif, the price is in the Serif font, and the description is in a smaller, lighter-weight sans-serif. Use a thin horizontal rule between items.