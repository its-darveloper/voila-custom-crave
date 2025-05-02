# Voila Custom Crave

A custom Shopify theme based on Dawn, featuring biophilic design elements and enhanced user experience with a nature-inspired approach.

[Features](#features) |
[Design Philosophy](#design-philosophy) |
[Getting Started](#getting-started) |
[Customization](#customization) |
[Accessibility](#accessibility) |
[Development](#development)

## Features

Voila Custom Crave extends Dawn's HTML-first approach while incorporating modern biophilic design elements:

* **Nature-Inspired Navigation:** Enhanced mega menus and dropdowns with organic shapes, natural motion, and warm earth-tone colors
* **Biophilic Elements:** Leaf patterns, natural textures, and a color palette derived from nature
* **Enhanced Accessibility:** WCAG-compliant contrast ratios, reduced motion options, and improved keyboard navigation
* **Human-Centered Design:** Intuitive information architecture and thoughtful interaction patterns
* **Micro-Interactions:** Subtle animations that enhance user experience without being distracting
* **Responsive & Fast:** Maintains Dawn's performance focus while adding visual richness

## Design Philosophy

The theme is built around these core design principles:

### Biophilic Design

Biophilic design connects users with nature through:
- Organic shapes and patterns
- Nature-inspired color palettes
- Natural textures and visual elements
- Balanced white space mimicking natural environments

### Human-Centered

Every design decision puts the user first:
- Clear visual hierarchy and intuitive navigation
- Reduced cognitive load with thoughtful information architecture
- Consistent interaction patterns that feel natural
- Design choices that support emotional well-being

### Accessibility

Built for everyone, regardless of ability:
- High contrast text meeting WCAG AA standards
- Reduced motion options for vestibular sensitivity
- Keyboard navigable interfaces
- Screen reader optimized markup

## Getting Started

### Prerequisites
- Shopify Partner account
- Shopify CLI installed

### Installation

1. Clone the repository
```bash
git clone https://your-repository-url/voila-custom-crave.git
cd voila-custom-crave
```

2. Use Shopify CLI to preview
```bash
shopify theme serve
```

3. Deploy to a development store
```bash
shopify theme push
```

## Customization

The theme offers various customization options through the Theme Editor:

### Color Schemes
- **Warm Earth:** Warm beige (#f5efe0) base with forest green (#2a6e3f) accents
- **Nature's Calm:** Soft green base with earthy accent tones
- **Forest Light:** Light background with deep green highlights

### Navigation Options
- Standard dropdown with biophilic hover effects
- Enhanced mega menu with featured sections
- Mobile drawer navigation with organic transitions

### Animation Settings
- Animation intensity controls
- Reduced motion toggle for accessibility

## Accessibility

Voila Custom Crave prioritizes accessibility with:

- **Color Contrast:** All text meets WCAG 2.1 AA contrast requirements
- **Keyboard Navigation:** Complete keyboard control with visible focus states
- **Reduced Motion:** Alternative animations for users with vestibular sensitivity
- **Screen Reader Support:** Semantic HTML and ARIA attributes for assistive technologies

## Development

### Folder Structure

- `/assets`: CSS, JavaScript, and SVG files
- `/layout`: Theme layout templates
- `/sections`: Theme sections like header, footer, and product templates
- `/snippets`: Reusable code blocks
- `/templates`: Page templates

### Key Files

- `assets/component-mega-menu.css`: Enhanced mega menu styling
- `snippets/header-dropdown-menu.liquid`: Biophilic dropdown menu implementation
- `snippets/header-mega-menu.liquid`: Nature-inspired mega menu implementation

### Commands

Run Theme Check to validate your theme:
```bash
shopify theme check
```

Run Lighthouse to test performance:
```bash
npm install -g lighthouse
lighthouse https://your-store.myshopify.com
```

### Staying Up to Date

As this theme is based on Dawn, you can pull in upstream changes:

```bash
git remote add upstream https://github.com/Shopify/dawn.git
git fetch upstream
git merge upstream/main
```

## License

Based on Dawn by Shopify Inc. See [LICENSE](/LICENSE.md) for details.