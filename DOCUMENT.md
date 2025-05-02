# Voila Custom Crave: Theme Documentation

This document provides an overview of the key files and components in the Voila Custom Crave Shopify theme.

## Core File Structure

Voila Custom Crave follows the standard Shopify Online Store 2.0 theme architecture with the following main directories:

```
/
├── assets/           # CSS, JavaScript, and other static assets
├── config/           # Theme settings and schema definitions
├── layout/           # Main theme layouts
├── locales/          # Translation files
├── sections/         # Theme sections (modular, reusable components)
├── snippets/         # Reusable liquid code fragments
└── templates/        # Page templates
```

## Key Theme Files

### Layout Files

| File | Description |
|------|-------------|
| `layout/theme.liquid` | The main layout wrapper that contains the document structure, header, footer, and loads global CSS/JS |
| `layout/password.liquid` | Layout used when the store is password-protected |

### Main Configuration Files

| File | Description |
|------|-------------|
| `config/settings_schema.json` | Defines the structure of the theme editor settings |
| `config/settings_data.json` | Stores the actual theme settings values |

### Core JavaScript Files

| File | Description |
|------|-------------|
| `assets/global.js` | Core JavaScript functionality used throughout the site |
| `assets/constants.js` | Global constants used in JavaScript |
| `assets/animations.js` | Handles biophilic animations and transitions |
| `assets/cart.js` | Cart functionality and AJAX operations |

### Core CSS Files

| File | Description |
|------|-------------|
| `assets/base.css` | Base styling and CSS variables |
| `assets/component-mega-menu.css` | Biophilic mega menu styling |
| `assets/component-menu-drawer.css` | Mobile navigation drawer styling |
| `assets/component-cart-drawer.css` | Cart drawer styling |

### Navigation Components

| File | Description |
|------|-------------|
| `snippets/header-dropdown-menu.liquid` | Biophilic dropdown menu implementation |
| `snippets/header-mega-menu.liquid` | Enhanced nature-inspired mega menu |
| `snippets/header-drawer.liquid` | Mobile navigation drawer |
| `sections/header.liquid` | Main header section that incorporates navigation components |

### Product Components

| File | Description |
|------|-------------|
| `sections/main-product.liquid` | Main product template section |
| `snippets/product-media-gallery.liquid` | Product images and media gallery |
| `snippets/product-variant-picker.liquid` | Product variant selection interface |
| `snippets/price.liquid` | Price display with sale and compare-at functionality |

### Cart Components

| File | Description |
|------|-------------|
| `snippets/cart-drawer.liquid` | Cart drawer implementation |
| `sections/cart-drawer.liquid` | Cart drawer section wrapper |
| `sections/main-cart-items.liquid` | Cart page items listing |
| `sections/main-cart-footer.liquid` | Cart totals and checkout buttons |

### Collection Components

| File | Description |
|------|-------------|
| `sections/main-collection-product-grid.liquid` | Collection product grid display |
| `snippets/card-product.liquid` | Individual product card in collections |
| `snippets/facets.liquid` | Collection filtering and sorting |

## Customized Biophilic Elements

The following files contain our custom biophilic design implementation:

### Navigation

| File | Description |
|------|-------------|
| `assets/component-mega-menu.css` | Biophilic styling for mega menu with nature-inspired colors and patterns |
| `snippets/header-dropdown-menu.liquid` | Enhanced dropdown with organic interactions |
| `snippets/header-mega-menu.liquid` | Nature-inspired mega menu with featured sections |

### Component Styling

| File | Description |
|------|-------------|
| `assets/component-card.css` | Product card styling with organic transitions |
| `assets/component-slider.css` | Enhanced slider with natural motion physics |
| `assets/component-buttons.css` | Button styling with biophilic hover effects |

### Animation and Interactions

| File | Description |
|------|-------------|
| `assets/animations.js` | JavaScript for biophilic animations with reduced motion alternatives |
| `assets/details-disclosure.js` | Enhanced accordion and disclosure components |

## Theme Configuration

### Color Schemes

The theme includes several nature-inspired color schemes defined in `config/settings_schema.json`:

- **Warm Earth:** Warm beige (#f5efe0) with forest green (#2a6e3f) accents
- **Nature's Calm:** Soft green base with earthy accent tones
- **Forest Light:** Light background with deep green highlights

The CSS variables for these schemes are defined in:
- `layout/theme.liquid` (CSS variables in the `<style>` block)
- Individual component CSS files

### Typography

Typography settings focus on readability and natural rhythm with:
- Balanced font scales
- Optimal line heights
- Responsive sizing

## Accessibility Features

| Feature | Implementation |
|---------|----------------|
| Reduced Motion | `@media (prefers-reduced-motion: reduce)` rules in CSS |
| Color Contrast | High contrast text meeting WCAG AA standards |
| Keyboard Navigation | Enhanced focus states and logical tab order |
| Screen Reader | ARIA attributes and semantic HTML |

## Custom SVG Icons

The theme includes a set of custom nature-inspired SVG icons in the `assets/` directory, including:
- Leaf icons for navigation
- Organic shapes for UI elements
- Natural pattern elements

## Performance Optimizations

- Critical CSS inlining in `layout/theme.liquid`
- Lazy-loading images and non-critical CSS
- Deferred JavaScript loading
- Image optimization

## How to Customize

### Modifying the Navigation

1. Edit mega menu styling in `assets/component-mega-menu.css`
2. Modify menu structure in `snippets/header-mega-menu.liquid` and `snippets/header-dropdown-menu.liquid`

### Changing Color Schemes

1. Edit CSS variables in the `<style>` block in `layout/theme.liquid`
2. Update color scheme definitions in `config/settings_schema.json`

### Adding New Components

1. Create a new section file in the `sections/` directory
2. Register it in the schema at the bottom of the file
3. Add CSS styling in the `assets/` directory