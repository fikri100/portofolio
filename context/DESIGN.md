---
name: Modern Engineer Portfolio
colors:
  surface: '#131315'
  surface-dim: '#131315'
  surface-bright: '#39393b'
  surface-container-lowest: '#0e0e10'
  surface-container-low: '#1c1b1d'
  surface-container: '#201f22'
  surface-container-high: '#2a2a2c'
  surface-container-highest: '#353437'
  on-surface: '#e5e1e4'
  on-surface-variant: '#dfbec3'
  inverse-surface: '#e5e1e4'
  inverse-on-surface: '#313032'
  outline: '#a7898d'
  outline-variant: '#584144'
  surface-tint: '#ffb2bf'
  primary: '#ffb2bf'
  on-primary: '#660027'
  primary-container: '#f65881'
  on-primary-container: '#5a0021'
  inverse-primary: '#b22350'
  secondary: '#ffb4ab'
  on-secondary: '#670508'
  secondary-container: '#8a221d'
  on-secondary-container: '#ff9f94'
  tertiary: '#d2bbff'
  on-tertiary: '#3f008e'
  tertiary-container: '#a476ff'
  on-tertiary-container: '#36007d'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffd9de'
  primary-fixed-dim: '#ffb2bf'
  on-primary-fixed: '#3f0015'
  on-primary-fixed-variant: '#90003a'
  secondary-fixed: '#ffdad6'
  secondary-fixed-dim: '#ffb4ab'
  on-secondary-fixed: '#410002'
  on-secondary-fixed-variant: '#87201b'
  tertiary-fixed: '#eaddff'
  tertiary-fixed-dim: '#d2bbff'
  on-tertiary-fixed: '#25005a'
  on-tertiary-fixed-variant: '#5a00c6'
  background: '#131315'
  on-background: '#e5e1e4'
  surface-variant: '#353437'
typography:
  display-lg:
    fontFamily: Montserrat
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Montserrat
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg-mobile:
    fontFamily: Montserrat
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Montserrat
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 1200px
  gutter: 24px
  margin-desktop: 80px
  margin-mobile: 24px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
  section-gap: 120px
---

## Brand & Style

This design system is built for a software engineer who balances technical rigor with creative execution. The brand personality is **sophisticated, precise, and approachable**, aiming to evoke trust in the user's technical capabilities while showcasing a modern, design-literate sensibility.

The visual direction follows a **Minimalist-Glassmorphic hybrid** style. It utilizes heavy whitespace and a refined dark-mode foundation to allow high-vibrancy gradients to serve as focal points. The aesthetic is "polished developer"—meaning it avoids unnecessary clutter in favor of clean lines, functional clarity, and subtle depth that mimics a high-end IDE or modern SaaS dashboard.

## Colors

The palette is anchored by a **Rose Pink to Deep Coral gradient**, directly inspired by the engineer’s signature visual identity. This gradient is used sparingly for primary actions, accents, and decorative elements to maintain a professional "tech-forward" atmosphere.

- **Primary & Secondary:** Used for "Power Gradients" on buttons, active states, and decorative typography.
- **Neutral:** A deep Zinc/Slate scale provides the foundation. Pure blacks are avoided in favor of slightly tinted charcoals to reduce eye strain and improve the perceived quality of shadows.
- **Accents:** Tertiary violet is used for syntax highlighting or category tags to differentiate technical skills from general content.

## Typography

The typography strategy pairs the geometric strength of **Montserrat** for display roles with the utilitarian precision of **Inter** for long-form content.

- **Headlines:** Use Montserrat with tight letter-spacing and bold weights to create a sense of confidence and "impact."
- **Body:** Inter is set with generous line-height (1.5x - 1.6x) to ensure maximum readability during deep dives into project descriptions or technical experience.
- **Labels:** Small caps and increased tracking are applied to metadata (e.g., dates, categories) to create a clear architectural hierarchy.

## Layout & Spacing

The layout utilizes a **12-column fluid grid** with a fixed maximum width to ensure content remains readable on ultra-wide monitors. 

- **Generous Margins:** Section transitions are defined by significant vertical breathing room (120px+) to evoke a "high-end gallery" feel.
- **Rhythm:** An 8px base unit governs all internal component spacing.
- **Reflow:** On mobile devices, margins shrink to 24px, and 12-column layouts collapse into a single vertical stack. Grid gutters remain constant to maintain visual consistency in cards and lists.

## Elevation & Depth

Hierarchy in this design system is achieved through **Tonal Layering** and **Glassmorphism**, rather than heavy traditional shadows.

1.  **Level 0 (Base):** The primary background color.
2.  **Level 1 (Cards):** Slightly lighter surface color with a 1px low-opacity border (white at 10% opacity) to define edges against the dark background.
3.  **Level 2 (Overlays):** Semi-transparent surfaces with a `backdrop-filter: blur(12px)`. This is used for navigation bars and modal windows.
4.  **Shadows:** When used, shadows are "Ambient"—extremely diffused, large radius (32px+), and low opacity (15-20%), serving as a soft glow rather than a hard drop shadow.

## Shapes

The design system employs **Level 2 (Rounded)** shapes. This moderate corner radius balances the "tech" feel (which can be too sharp) with a modern "friendly" approachable vibe.

- **Small elements (Chips/Tags):** Use a 4px radius.
- **Standard elements (Buttons/Inputs):** Use an 8px radius.
- **Large elements (Cards/Sections):** Use a 16px radius.
- **Interactive containers:** Maintain consistent nesting; inner elements should have a smaller radius than their parent containers to maintain visual harmony.

## Components

### Buttons
- **Primary:** Gradient background (Rose to Coral), white text, 8px radius. On hover, a subtle scale-up (1.02x) and an increase in the outer glow/shadow brightness.
- **Secondary:** Transparent background with a 1px gradient border. Text remains white or primary pink.

### Project Cards
- Constructed with a Level 1 surface. 
- Features a "glass" header for the project title.
- Imagery should use `object-fit: cover` with a slight zoom effect on card hover.

### Skill Chips
- Low-contrast background (Zinc-800) with Montserrat bold labels in 12px.
- Use primary color for "Core" skills and secondary for "Supporting" skills.

### Form Inputs
- Dark background, 1px border. 
- The border transitions to the primary gradient upon focus.
- Use Inter for input text to ensure technical characters (like in email addresses) are distinct.

### Experience Timeline
- A vertical 2px line using a muted gradient. 
- Chronological nodes use the primary pink color with a soft outer glow to signify "activity."