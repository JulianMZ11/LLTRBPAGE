---
name: Obsidian High-Contrast
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f4'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#4c4546'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f0f1f1'
  outline: '#7e7576'
  outline-variant: '#cfc4c5'
  surface-tint: '#5e5e5e'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1b1b1b'
  on-primary-container: '#848484'
  inverse-primary: '#c6c6c6'
  secondary: '#5e5e5e'
  on-secondary: '#ffffff'
  secondary-container: '#e2e2e2'
  on-secondary-container: '#646464'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1b1b1b'
  on-tertiary-container: '#848484'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c6'
  on-primary-fixed: '#1b1b1b'
  on-primary-fixed-variant: '#474747'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c6'
  on-secondary-fixed: '#1b1b1b'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1b1b1b'
  on-tertiary-fixed-variant: '#474747'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
  pure-black: '#000000'
  pure-white: '#FFFFFF'
  stroke-gray: '#E5E5E5'
  surface-subtle: '#F9F9F9'
typography:
  display:
    fontFamily: metropolis
    fontSize: 72px
    fontWeight: '800'
    lineHeight: 80px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: metropolis
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: metropolis
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 38px
  headline-md:
    fontFamily: metropolis
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: jetbrainsMono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: jetbrainsMono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.08em
spacing:
  unit: 8px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  max-width: 1280px
---

## Brand & Style
This design system utilizes a high-contrast, minimalist aesthetic that leans into a "Digital Noir" or "Hyper-Clean" personality. It is designed for high-density information environments where clarity and authority are paramount. The target audience includes developers, architects, and data analysts who value efficiency over decoration.

The design style is **Minimalist-Brutalist**: it uses a strictly monochromatic palette, razor-sharp edges, and heavy use of whitespace to create a rhythmic, structured experience. By removing the distraction of color, the focus is placed entirely on content hierarchy and functional interactions.

## Colors
The palette is intentionally restricted to absolute extremes: Pure Black (#000000) and Pure White (#FFFFFF). 

- **Primary & Secondary:** Both are mapped to black to ensure that every call-to-action and meaningful stroke has maximum visual weight.
- **Backgrounds:** Use pure white for the main canvas to maintain high brightness and readability.
- **Functional Grays:** A very limited scale of "ink" grays is permitted only for borders and secondary metadata to prevent the UI from feeling flat, but these should be used sparingly.

## Typography
The typography system provides the "texture" of the brand. We replace generic system fonts with a more structured trio:

1.  **Metropolis** for headlines: A geometric sans-serif that provides a modern, architectural feel.
2.  **Inter** for body text: Highly legible and neutral, optimized for screen reading.
3.  **JetBrains Mono** for labels: A monospaced font used for data points, tags, and small technical labels to emphasize the "built" nature of the interface.

All caps should be applied to `label-sm` and `label-md` to create a "technical blueprint" aesthetic.

## Layout & Spacing
The layout follows a **Fixed Grid** philosophy on desktop and a **Fluid** model on mobile.

- **Grid:** Use a 12-column grid for desktop (1280px max-width) with 24px gutters. On mobile, transition to a 4-column fluid grid.
- **Rhythm:** All spacing must be a multiple of 8px. Use large vertical gaps (80px, 120px) between major sections to emphasize the minimalist aesthetic.
- **Alignment:** Strictly align all elements to the left margin. Avoid centered layouts unless it is a dedicated splash page.

## Elevation & Depth
In this design system, depth is conveyed through **Bold Borders** and **Tonal Layers** rather than shadows.

- **No Shadows:** Do not use box-shadows or blurs. 
- **Borders:** Use 1px or 2px solid black strokes to define containers.
- **Tonal Stepping:** Use `#F9F9F9` to distinguish nested containers or "wells" within a white page.
- **Negative Space:** Use empty space as the primary method of separation. Elements should feel like they are floating in a vacuum or locked into a rigid grid.

## Shapes
The shape language is strictly **Sharp (0px)**. 

Every element—from buttons and input fields to cards and modal windows—must have 90-degree corners. This reinforces the Brutalist and technical nature of the system. There are no exceptions for "pill" shapes or rounded icons; icons should also feature sharp terminals where possible.

## Components
- **Buttons:** Solid black background with white text for primary actions. 1px black outline with white background for secondary. No rounded corners. Use `label-md` for button text.
- **Input Fields:** 1px black bottom-border only (minimalist style) or full 1px box. Active state is signaled by a 2px stroke.
- **Chips/Tags:** Use `label-sm` in all caps. 1px black border, white background.
- **Cards:** 1px solid black border. No shadow. Ensure generous internal padding (32px) to maintain the minimalist feel.
- **Lists:** Separated by 1px horizontal lines (`#E5E5E5`). Use monospaced numbers for ordered lists.
- **Checkboxes:** Square, black fill when selected. Use a simple "X" or a minimalist checkmark.
- **Navigation:** Top-aligned, text-only navigation using `label-md`. Use bold weights or a simple underline for active states.