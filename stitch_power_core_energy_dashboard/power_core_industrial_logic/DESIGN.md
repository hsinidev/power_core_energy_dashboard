---
name: Power-Core Industrial Logic
colors:
  surface: '#1d100a'
  surface-dim: '#1d100a'
  surface-bright: '#46362e'
  surface-container-lowest: '#170b06'
  surface-container-low: '#261812'
  surface-container: '#2b1c16'
  surface-container-high: '#362720'
  surface-container-highest: '#41312a'
  on-surface: '#f8ddd2'
  on-surface-variant: '#e2bfb0'
  inverse-surface: '#f8ddd2'
  inverse-on-surface: '#3d2d26'
  outline: '#a98a7d'
  outline-variant: '#5a4136'
  surface-tint: '#ffb693'
  primary: '#ffb693'
  on-primary: '#561f00'
  primary-container: '#ff6b00'
  on-primary-container: '#572000'
  inverse-primary: '#a04100'
  secondary: '#c6c6c7'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#c8c6c5'
  on-tertiary: '#313030'
  tertiary-container: '#9a9898'
  on-tertiary-container: '#313131'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdbcc'
  primary-fixed-dim: '#ffb693'
  on-primary-fixed: '#351000'
  on-primary-fixed-variant: '#7a3000'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c6c7'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#e5e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1c1b1b'
  on-tertiary-fixed-variant: '#474746'
  background: '#1d100a'
  on-background: '#f8ddd2'
  surface-variant: '#41312a'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  body-base:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0.01em
  data-mono:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
spacing:
  unit: 4px
  gutter: 16px
  margin: 24px
  container-max: 1440px
  border-thick: 2px
  border-heavy: 4px
---

## Brand & Style

This design system is built on a foundation of **Industrial Brutalism** and **Tactical Utility**. It is designed for high-stakes environments where clarity, durability, and immediate data density are paramount. The aesthetic rejects decorative softness in favor of structural honesty, mimicking the physical chassis of high-end power hardware.

The emotional response should be one of absolute reliability and technical precision. Every interface element is treated as a physical component—latched, bolted, or etched into the layout. High-contrast boundaries and a rigid adherence to a grid ensure that the user feels in control of a powerful, complex machine.

## Colors

The palette is anchored by **Safety Orange**, used strictly for interactive elements, critical alerts, and branding highlights to ensure maximum visibility against the **Charcoal** environment. The background utilizes a near-black (#0D0D0D) to minimize eye strain in low-light field conditions and to make data "pop" like a glowing vacuum fluorescent display.

**White** is reserved for high-priority data readouts and labels. Semantic colors (Success, Warning, Error) follow industrial lighting standards: high-saturation tones that cut through the dark UI. Surface variations are subtle, using shades of Charcoal to define physical depth without relying on shadows.

## Typography

The typography strategy leverages **Space Grotesk** for structural headlines to provide a technical, geometric edge. **Inter** is utilized for all functional text and data displays due to its exceptional legibility and high x-height.

Data visualization and numerical readouts should utilize the Bold weights of Inter with increased letter spacing to mimic the look of etched hardware labels. All labels for buttons and inputs must be set in All-Caps to reinforce the "industrial control" aesthetic.

## Layout & Spacing

This design system employs a **Rigid Grid** model. All layouts are based on a 4px baseline unit and a strict 12-column grid for desktop. Containers do not use soft padding; instead, they use "Inset Zones" defined by thick internal borders.

Components are packed tightly to allow for high data density, reflecting a professional dashboard. Content should be grouped in modular "Blocks" that resemble rack-mounted equipment. Gutters are kept narrow (16px) to maintain a cohesive, monolithic feel.

## Elevation & Depth

Elevation is conveyed through **Physical Layering and Bold Borders** rather than shadows. This design system treats the Z-axis as a series of stacked plates.

- **Level 0 (Base):** The darkest surface (#0D0D0D).
- **Level 1 (Panels):** Charcoal surfaces (#1A1A1A) with a 2px solid border (#262626).
- **Level 2 (Interactive):** Buttons and active inputs, outlined with Safety Orange or high-contrast White.
- **Active State:** Elements should "illuminate" (using a 0px blur, high-spread outer glow in the primary color) to simulate a backlit hardware button.

Shadows are avoided entirely to maintain the flat, rugged, industrial aesthetic.

## Shapes

The shape language is strictly **Geometric and Sharp**. A 0px corner radius is applied to all components, containers, and buttons to evoke the feeling of machined metal and precision-cut components.

Exceptions are made only for status indicators (LED pips) which should be perfect circles or 45-degree chamfered octagons to simulate physical indicator lights.

## Components

### Buttons (Tactical)
Buttons must feel heavy. Use a 2px solid border. The 'Primary' variant uses a solid Safety Orange fill with Black text. The 'Secondary' variant is ghost-styled with a White border and White text. Hover states should trigger a color inversion or a solid fill "flash."

### Data Cards
Cards are the primary container for metrics. Each card must have a "Header Bar" (a solid 24px tall strip) containing the label in All-Caps. Data values should be displayed in the center in a large, bold weight.

### Inputs & Toggles
Input fields should look like recessed slots in a panel. Use a dark background with a 2px bottom-border only. Toggles should resemble heavy-duty rocker switches or physical sliders with high-contrast "On" states in Safety Orange.

### Status Pips
Small circular indicators used next to labels to indicate system health. Use a "Glow" effect (CSS drop-shadow) only on these elements to simulate an active LED.

### Progress Gauges
Instead of rounded progress bars, use segmented blocks. Each segment represents 5-10% of the total, creating a "Digital-Analog" readout aesthetic common in industrial machinery.