---
name: Augmented Robotics Interface
colors:
  surface: '#12121f'
  surface-dim: '#12121f'
  surface-bright: '#383846'
  surface-container-lowest: '#0d0d1a'
  surface-container-low: '#1a1a28'
  surface-container: '#1e1e2c'
  surface-container-high: '#292937'
  surface-container-highest: '#343342'
  on-surface: '#e3e0f3'
  on-surface-variant: '#bec7d3'
  inverse-surface: '#e3e0f3'
  inverse-on-surface: '#2f2f3d'
  outline: '#88929d'
  outline-variant: '#3e4852'
  surface-tint: '#95ccff'
  primary: '#95ccff'
  on-primary: '#003352'
  primary-container: '#00a8ff'
  on-primary-container: '#003a5c'
  inverse-primary: '#006399'
  secondary: '#d7ffc5'
  on-secondary: '#053900'
  secondary-container: '#2ff801'
  on-secondary-container: '#0f6d00'
  tertiary: '#ffba38'
  on-tertiary: '#432c00'
  tertiary-container: '#d49400'
  on-tertiary-container: '#4b3200'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#cde5ff'
  primary-fixed-dim: '#95ccff'
  on-primary-fixed: '#001d32'
  on-primary-fixed-variant: '#004a75'
  secondary-fixed: '#79ff5b'
  secondary-fixed-dim: '#2ae500'
  on-secondary-fixed: '#022100'
  on-secondary-fixed-variant: '#095300'
  tertiary-fixed: '#ffdeac'
  tertiary-fixed-dim: '#ffba38'
  on-tertiary-fixed: '#281900'
  on-tertiary-fixed-variant: '#604100'
  background: '#12121f'
  on-background: '#e3e0f3'
  surface-variant: '#343342'
typography:
  display-lg:
    fontFamily: Orbitron
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: 0.1em
  headline-lg:
    fontFamily: Orbitron
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  headline-md:
    fontFamily: Orbitron
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.2'
  body-lg:
    fontFamily: IBM Plex Mono
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: IBM Plex Mono
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-lg:
    fontFamily: Rajdhani
    fontSize: 16px
    fontWeight: '600'
    lineHeight: '1'
  label-sm:
    fontFamily: Rajdhani
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.2em
  headline-lg-mobile:
    fontFamily: Orbitron
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
spacing:
  unit: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  panel-padding: 20px
---

## Brand & Style
The design system is an immersive, AR-inspired interface designed to evoke the technical precision of high-end robotics engineering. It draws heavily from HUD (Heads-Up Display) aesthetics, blending functional data density with a futuristic, holographic atmosphere.

The style is **Cyber-Industrial Minimalism**. It avoids heavy gradients and skeuomorphism in favor of high-contrast line work, "glass" panels, and glowing optical effects. The goal is to make the user feel like they are operating a specialized terminal or wearing an AR visor while sourcing components for their exo-frame. 

Key visual identifiers include:
- **Optical Precision:** Heavy use of hair-thin lines, crosshairs, and measurement markers.
- **Holographic Depth:** Layers are defined by varying levels of transparency and glow rather than traditional drop shadows.
- **Systemic Feedback:** UI elements react with "pulse" animations and color shifts to simulate a live, data-driven environment.

## Colors
The palette is rooted in a deep "Matte Black" void to allow the neon accents to pop with maximum luminosity. 

- **Electric Blue (Primary):** Used for navigation, primary CTAs, and active "HUD" focus states.
- **Neon Green (Data):** Reserved for technical specifications, stock availability, and successful system confirmations.
- **Steel Grey (Surface):** The structural color for containers and panels, typically applied with low opacity to create a layered "glass" effect.
- **Warning Amber & Deep Crimson:** High-urgency colors for alerts, critical warnings, or out-of-stock indicators.

All accent colors should be paired with a matching `box-shadow` or `text-shadow` using a 15-25% opacity blur to simulate a digital glow.

## Typography
The typographic hierarchy prioritizes readability and technical flavor. 

- **Headlines (Orbitron):** Used for main product titles and section headers. Its mechanical geometry reinforces the robotics theme. Always use a slight letter spacing to prevent it from feeling cramped.
- **Body (IBM Plex Mono):** Used for all descriptions and technical data. The monospaced nature ensures that columns of numbers and specifications align perfectly, mimicking a terminal readout.
- **Labels (Rajdhani):** A condensed, clean sans-serif used for tags, button text, and metadata. It provides a sharp contrast to the more decorative Orbitron and the utilitarian IBM Plex Mono.

## Layout & Spacing
The layout follows a **Rigid Grid System** inspired by technical blueprints. 

- **Grid:** A 12-column layout for desktop with 24px gutters. Elements should ideally align to a 4px baseline grid to maintain "engineered" precision.
- **Scanlines:** A global overlay of 1px horizontal lines with 3% opacity should be applied to the entire viewport to simulate an old-school CRT or AR visor display.
- **Margins:** Generous outer margins (64px+) on desktop focus the user's attention on the central "HUD" data panels. 
- **Adaptation:** On mobile, complex side-panels collapse into "Drawers" accessed via bracketed icons. Typography scales down significantly to ensure technical tables remain legible.

## Elevation & Depth
This design system avoids soft drop shadows. Instead, it uses **Luminous Layering**:

1.  **Level 0 (Background):** Pure #0D0D0D with a subtle grid pattern (1px dots every 40px).
2.  **Level 1 (Panels):** Steel Grey (#2C2C3A) at 40% opacity with a `backdrop-filter: blur(10px)`. These panels have a 1px border of the same color.
3.  **Level 2 (Active Elements):** Elements in focus or hovered receive a 1px Electric Blue border and an outer glow (`box-shadow: 0 0 10px rgba(0, 168, 255, 0.3)`).
4.  **Level 3 (Pop-ups/Modals):** Full opacity panels with bright corner brackets to signify they have "broken" the standard HUD plane.

## Shapes
The shape language is strictly **Geometric and Angular**. 

- **Corner Brackets:** Instead of full borders, many containers should use corner-only brackets (top-left and bottom-right) to define their boundaries.
- **Beveled Edges:** Larger structural panels may feature "clipped" corners (45-degree cuts) at 8px to mimic industrial plating.
- **No Curves:** Rounded corners are prohibited in this design system to maintain the aggressive, mechanical aesthetic.

## Components
- **Buttons:** Styled as `[ COMMAND ]`. They feature a transparent background and a 1px border. On hover, the background fills with Electric Blue (30% opacity) and the text glows.
- **Input Fields:** Bottom-border only, or 1px border with the left and right sides featuring "bracket" extensions. The cursor should be a solid, blinking block.
- **Chips/Status Badges:** Small rectangular blocks with no roundedness. Active states should use the Neon Green palette. 
- **Cards:** Product cards must include a "crosshair" in the center of the image area that only appears on hover. Text within cards should be categorized with small Label-sm headers (e.g., "PART_NO: 88-X").
- **Checkboxes/Radios:** Square frames. Checkboxes use an "X" mark instead of a tick to maintain the technical readout feel.
- **Progress Bars:** Segmented blocks (stepped) rather than a continuous smooth fill, evoking battery or power indicators.