# Design Tokens

## Overview

SC Design System uses a comprehensive set of design tokens to maintain consistency across all components and layouts. These tokens are defined in both JSON and SCSS formats for maximum flexibility.

## Color Tokens

Our color system is based on Material Design 3 principles with StellantAI brand colors.

```json
{
  "colors": {
    "primary": {
      "50": "#E8F5E9",
      "100": "#C8E6C9",
      "500": "#4CAF50",
      "700": "#388E3C"
    },
    "neutral": {
      "50": "#FAFAFA",
      "100": "#F5F5F5",
      "200": "#EEEEEE",
      "300": "#E0E0E0"
    }
  }
}
```

## Typography

Font families and scales are defined to ensure consistent text hierarchy.

```scss
$font-family-base: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
$font-size-base: 16px;
$line-height-base: 1.5;
```

## Spacing

Consistent spacing scale for margins and padding.

```scss
$spacing-unit: 8px;
$spacing-scale: (
  'xs': $spacing-unit,
  'sm': $spacing-unit * 2,
  'md': $spacing-unit * 3,
  'lg': $spacing-unit * 4,
  'xl': $spacing-unit * 6
);
```

## Usage

Design tokens can be accessed through:

1. SCSS variables in your stylesheets
2. JSON files for JavaScript applications
3. CSS custom properties for runtime theming 