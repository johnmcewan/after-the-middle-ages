---
name: Medieval Scholarly System
colors:
  surface: '#fcf9ee'
  surface-dim: '#dddacf'
  surface-bright: '#fcf9ee'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f7f4e9'
  surface-container: '#f1eee3'
  surface-container-high: '#ebe8dd'
  surface-container-highest: '#e5e2d8'
  on-surface: '#1c1c15'
  on-surface-variant: '#43474c'
  inverse-surface: '#31312a'
  inverse-on-surface: '#f4f1e6'
  outline: '#74777d'
  outline-variant: '#c4c6cd'
  surface-tint: '#4d6076'
  primary: '#001022'
  on-primary: '#ffffff'
  primary-container: '#12263a'
  on-primary-container: '#7a8ea6'
  inverse-primary: '#b5c8e2'
  secondary: '#7b5811'
  on-secondary: '#ffffff'
  secondary-container: '#fdcd7c'
  on-secondary-container: '#78550e'
  tertiary: '#2a0001'
  on-tertiary: '#ffffff'
  tertiary-container: '#520105'
  on-tertiary-container: '#dc695f'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d0e4ff'
  primary-fixed-dim: '#b5c8e2'
  on-primary-fixed: '#071d30'
  on-primary-fixed-variant: '#35485e'
  secondary-fixed: '#ffdeaa'
  secondary-fixed-dim: '#eebf70'
  on-secondary-fixed: '#271900'
  on-secondary-fixed-variant: '#5f4100'
  tertiary-fixed: '#ffdad6'
  tertiary-fixed-dim: '#ffb4ac'
  on-tertiary-fixed: '#410002'
  on-tertiary-fixed-variant: '#822621'
  background: '#fcf9ee'
  on-background: '#1c1c15'
  surface-variant: '#e5e2d8'
typography:
  display-lg:
    fontFamily: notoSerif
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: notoSerif
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: notoSerif
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: newsreader
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: newsreader
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: newsreader
    fontSize: 13px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.08em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1140px
  gutter: 32px
  margin: 48px
  stack-sm: 16px
  stack-md: 32px
  stack-lg: 64px
---

## Brand & Style

The design system is rooted in the concept of the "Living Archive." It aims to evoke the atmosphere of a prestigious university scriptorium—quiet, authoritative, and deeply intellectual. The target audience includes historians, researchers, and cultural enthusiasts who value rigour and heritage.

The visual style is **Tactile Minimalism**. It balances the rich textures of historical artifacts with the functional clarity of modern academic publishing. By combining physical metaphors, such as paper grain and wax impressions, with a disciplined use of whitespace, the design system achieves a sense of "historical modernism." It feels like a contemporary digital window into a medieval world, prioritizing legiveness without sacrificing its atmospheric soul.

## Colors

The palette is derived from natural pigments and materials found in medieval manuscripts. 

*   **Deep Ink Blue:** Used for primary navigation, headings, and high-emphasis text. It represents the permanence of scribe ink.
*   **Antique Gold:** Reserved for accents, interactive states, and decorative flourishes (like drop caps or borders). It signifies prestige and illumination.
*   **Parchment Creams:** The foundation of the system. These off-whites reduce eye strain compared to pure white and provide a subtle organic texture to all backgrounds.
*   **Oxblood Red (Tertiary):** Used sparingly for critical alerts or "rubricated" text, mirroring the traditional red ink used for highlighting key passages in codices.

## Typography

Typography in this design system is treated with the reverence of a master typesetter.

*   **Headlines:** Using Noto Serif, headings are set with generous leading and a focus on hierarchical clarity. Display sizes should occasionally use italic weights to emphasize scholarly distinction.
*   **Body Text:** Newsreader provides the high legibility required for long-form academic abstracts. The x-height is optimized for screen reading while maintaining a literary character.
*   **Labels:** Small caps and increased letter-spacing are used for metadata, such as date, location, or "Document Type," to differentiate secondary information from the narrative body.

## Layout & Spacing

The layout philosophy follows a **Fixed Grid** model, reminiscent of a printed folio or an open book. 

A 12-column grid is utilized with wide margins to create a sense of focus and breathability. Content should be centered with significant "white space" (parchment space) to allow the eye to rest. Vertical rhythm is strictly enforced using an 8px baseline to ensure that blocks of text maintain the structured appearance of a manuscript. Elements should feel "anchored" to the page rather than floating.

## Elevation & Depth

Depth is conveyed through **Tonal Layers** and subtle tactile effects rather than heavy shadows.

*   **Paper Stacking:** Higher elevation is represented by layering a slightly lighter parchment tone over a darker one, often accompanied by a very thin (0.5px) dark-blue border to simulate the edge of a page.
*   **Embossing:** Buttons and interactive cards use inner shadows or "letterpress" effects to appear as if they are stamped into the parchment.
*   **Wax Seal Depth:** High-priority buttons or calls-to-action utilize a subtle radial gradient and a soft, tinted drop shadow to mimic the physical thickness of a wax seal pressed onto a surface.

## Shapes

The shape language is primarily **Soft (0.25rem)**, reflecting the natural, slightly rounded corners of hand-cut parchment and aged paper. 

Completely sharp corners (0px) are used for structural lines and separators to maintain an architectural, academic feel. However, containers and interactive elements use the 'Soft' radius to avoid appearing too industrial or aggressive. Wax-seal inspired elements (like "Save" buttons or badges) may use circular shapes to break the rigid grid and add a touch of organic character.

## Components

*   **Buttons:** Primary buttons are filled with Deep Ink Blue with Gold text. Secondary buttons are "Ghost" style with a 1px Gold border. All buttons use a transition that mimics the slight shimmer of metallic ink when hovered.
*   **Cards:** Research paper cards feature a faint parchment texture background and a "Deckle Edge" (a subtle, irregular border) on the bottom edge.
*   **Chips/Tags:** Designed to look like small ribbon fragments or circular wax stamps. They use the Oxblood Red or Antique Gold to categorize session topics.
*   **Inputs:** Form fields are minimalist underlines (resembling ruled lines on a page) that turn Antique Gold when focused.
*   **Separators:** Horizontal rules are not simple lines; they should feature a small fleur-de-lis or a geometric knot in the center, rendered in Antique Gold.
*   **Special Component (The Seal):** A floating action button styled as a physical wax seal, used for the "Register" or "Submit" primary actions of the conference.