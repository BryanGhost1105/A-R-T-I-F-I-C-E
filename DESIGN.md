---
name: Artifice Gallery
description: Elite curatorial agency for contemporary art.
colors:
  primary: "#09090b"
  neutral-bg: "#f9fafb"
  neutral-text: "#09090b"
  neutral-muted: "#a1a1aa"
  border-light: "#e4e4e7"
  glass-bg: "rgba(255, 255, 255, 0.4)"
typography:
  display:
    fontFamily: "Instrument Sans, system-ui, sans-serif"
    fontSize: "clamp(3.2rem, 6.5vw, 7.5rem)"
    fontWeight: 500
    lineHeight: 0.85
    letterSpacing: "-0.05em"
  headline:
    fontFamily: "Instrument Sans, system-ui, sans-serif"
    fontSize: "clamp(1.8rem, 4.5vw, 4.8rem)"
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Instrument Sans, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 300
    lineHeight: 1.6
    letterSpacing: "normal"
rounded:
  full: "9999px"
  lg: "1rem"
  xl: "2.5rem"
spacing:
  xs: "0.5rem"
  sm: "1rem"
  md: "2rem"
  lg: "4rem"
components:
  nav-pill:
    backgroundColor: "{colors.glass-bg}"
    rounded: "{rounded.full}"
    padding: "14px 32px"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "#ffffff"
    rounded: "{rounded.full}"
    padding: "6px 24px"
  card-editorial:
    backgroundColor: "{colors.neutral-bg}"
    rounded: "{rounded.xl}"
    padding: "40px"
---

# Design System: Artifice Gallery

## 1. Overview

**Creative North Star: "The Cinematic Sanctuary"**

Artifice Gallery is an editorial, high-fidelity design system that simulates the experience of a physical vanguard gallery. It prioritizes depth, materiality, and structural precision. The aesthetic is defined by a monochromatic palette, generous whitespace, and layered motion that creates a sense of three-dimensional space.

**Key Characteristics:**
- **Layered Depth**: Use of glassmorphism, grain overlays, and parallax to create a spatial experience.
- **Typographic Authority**: Large, tightly tracked display type and editorial-grade body hierarchy.
- **Monochromatic Focus**: Color is rare and purposeful, used only to highlight art or specific actions.
- **Architectural Rhythm**: Asymmetrical layouts and bento grids that feel constructed, not templated.

## 2. Colors

The palette is strictly monochromatic, using tinted neutrals to avoid the "dead" feel of pure black and white.

### Primary
- **Vanguard Black** (#09090b): Used for authoritative typography, primary actions, and deep backgrounds.

### Neutral
- **Sanctuary White** (#f9fafb): The primary background color. It is a warm, slightly tinted neutral that reduces eye strain compared to pure white.
- **Muted Zinc** (#a1a1aa): Used for secondary labels, borders, and placeholders.
- **Glass White** (rgba(255, 255, 255, 0.4)): Used for the navigation pill and other layered surfaces.

### Named Rules
**The 10% Rule.** Saturated color or pure black should never occupy more than 10% of a brand surface unless in a "Drenched" state (like the footer). Silence is the default.

## 3. Typography

**Display Font:** Instrument Sans
**Body Font:** Instrument Sans

**Character:** Modern, clean, and highly legible. It carries an editorial weight that feels both timeless and vanguard.

### Hierarchy
- **Display** (Medium, clamp(3.2rem, 6.5vw, 7.5rem), 0.85): Used for primary hero headlines. Always lowercase or uppercase, never sentence case.
- **Headline** (Normal, clamp(1.8rem, 4.5vw, 4.8rem), 1.1): Used for the manifesto and section intros.
- **Title** (Medium, 1.875rem, 1.2): Used for card titles and sub-sections.
- **Body** (Light, 1rem, 1.6): Used for descriptive copy. Max line length capped at 40ch for readability.
- **Label** (Medium, 0.75rem, 0.4em tracking, uppercase): Used for navigation links and overlines.

## 4. Elevation

Artifice avoids standard drop shadows, preferring tonal layering and glassmorphism to convey depth.

### Named Rules
**The Structural Depth Rule.** Depth is created through stacking order and backdrop filters. Elements closer to the user are more translucent and have higher backdrop-blur values (3xl).

## 5. Components

### Navigation Pill
- **Shape:** Rounded Full (9999px)
- **Style:** Translucent glass (white/40) with a 3xl backdrop blur and a thin white border.
- **Hover:** Increases brightness and shadow depth.

### Primary Button
- **Shape:** Rounded Full (9999px)
- **Style:** Solid black background with white text. High tracking on uppercase labels.
- **Hover:** Slight scale down (0.98) and shadow increase.

### Editorial Card
- **Shape:** Rounded XL (2.5rem)
- **Style:** Usually contains a grayscale image with a subtle grain overlay.
- **Transition:** Scale up on hover (1.05) over 2 seconds for a cinematic feel.

## 6. Do's and Don'ts

### Do:
- **Do** use OKLCH for all new color definitions.
- **Do** cap body text line length at 40ch.
- **Do** use generous vertical spacing (32-56rem) between major sections.
- **Do** ensure all images have a subtle grayscale filter until hovered.

### Don't:
- **Don't** use standard "SaaS blue" or generic accent colors.
- **Don't** use nested cards or side-stripe borders.
- **Don't** use modals as a first-run interaction.
- **Don't** use pure `#000` or `#fff` without a tint.
 <!-- SEED -->
