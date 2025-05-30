# Griddock CSS Framework

A modern, lightweight CSS framework built entirely with **CSS Grid** instead of Flexbox. Griddock provides powerful, flexible layouts and a comprehensive component library inspired by Bulma, but leveraging the superior layout capabilities of CSS Grid.

## 🎯 Why Griddock?

- **CSS Grid First**: Built entirely with CSS Grid for more powerful and flexible layouts
- **Bulma-Inspired**: Familiar class naming and component structure for easy adoption
- **No JavaScript**: Pure CSS framework that works without any JavaScript dependencies
- **Lightweight**: Clean, efficient code with minimal overhead
- **Responsive**: Mobile-first design with comprehensive breakpoint utilities
- **Customizable**: CSS custom properties for easy theming and customization

## 🚀 Quick Start

### CDN (Coming Soon)
```html
<link rel="stylesheet" href="https://unpkg.com/griddock@latest/css/griddock.min.css">
```

### Download
1. Download `griddock.css` or `griddock.min.css` from the `css/` directory
2. Include it in your HTML:

```html
<link rel="stylesheet" href="path/to/griddock.css">
```

### NPM (Coming Soon)
```bash
npm install griddock
```

## 📖 Documentation

### Grid System

Griddock's grid system is built with CSS Grid, providing more powerful layouts than traditional flexbox-based frameworks.

#### Basic Grid
```html
<div class="grid is-3-columns">
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
</div>
```

#### Grid with Spans
```html
<div class="grid">
  <div class="span-8">Main content (8 columns)</div>
  <div class="span-4">Sidebar (4 columns)</div>
</div>
```

#### Responsive Grid
```html
<div class="grid is-mobile-1-column is-tablet-2-columns is-desktop-3-columns">
  <div>Responsive item 1</div>
  <div>Responsive item 2</div>
  <div>Responsive item 3</div>
</div>
```

### Container
Center your content with a responsive container:

```html
<div class="container">
  <p>Centered content with max-width</p>
</div>
```

### Components

#### Buttons
```html
<button class="button is-primary">Primary Button</button>
<button class="button is-large is-success">Large Success</button>
<button class="button is-outlined is-danger">Outlined Danger</button>
```

#### Cards
```html
<div class="card">
  <div class="card-header">
    <p class="card-header-title">Card Title</p>
  </div>
  <div class="card-content">
    <p>Card content goes here</p>
  </div>
  <div class="card-footer">
    <a class="card-footer-item">Save</a>
    <a class="card-footer-item">Edit</a>
  </div>
</div>
```

#### Forms
```html
<div class="field">
  <label class="label">Email</label>
  <input class="input" type="email" placeholder="Email address">
</div>

<div class="field">
  <label class="label">Message</label>
  <textarea class="textarea" placeholder="Your message"></textarea>
</div>

<div class="field is-grouped">
  <button class="button is-primary">Submit</button>
  <button class="button">Cancel</button>
</div>
```

#### Navigation
```html
<nav class="navbar is-primary">
  <div class="navbar-brand">
    <a class="navbar-item">Brand</a>
  </div>
  <div class="navbar-menu">
    <div class="navbar-start">
      <a class="navbar-item">Home</a>
      <a class="navbar-item">About</a>
    </div>
    <div class="navbar-end">
      <a class="navbar-item">Contact</a>
    </div>
  </div>
</nav>
```

### Utility Classes

#### Spacing
```html
<div class="m-4">Margin on all sides</div>
<div class="p-6">Padding on all sides</div>
<div class="mt-3 mb-5">Margin top and bottom</div>
```

#### Text
```html
<p class="has-text-primary">Primary colored text</p>
<p class="has-text-centered">Centered text</p>
<p class="has-text-weight-bold">Bold text</p>
```

#### Background Colors
```html
<div class="has-background-success">Success background</div>
<div class="has-background-light">Light background</div>
```

### Responsive Design

Griddock includes responsive utilities for different screen sizes:

- **Mobile**: `< 768px`
- **Tablet**: `768px - 1023px`
- **Desktop**: `1024px - 1215px`
- **Widescreen**: `1216px - 1407px`
- **Full HD**: `≥ 1408px`

#### Responsive Utilities
```html
<div class="is-hidden-mobile">Hidden on mobile</div>
<div class="is-hidden-tablet">Hidden on tablet</div>
<div class="grid is-mobile-1-column is-desktop-3-columns">
  <!-- 1 column on mobile, 3 on desktop -->
</div>
```

## 🎨 Customization

Griddock uses CSS custom properties for easy theming:

```css
:root {
  --primary: #your-primary-color;
  --secondary: #your-secondary-color;
  --success: #your-success-color;
  --grid-gap: 2rem;
  --container-max-width: 1400px;
  /* ... and many more */
}
```

## 🏗️ Building

To build the minified version:

```bash
npm install
npm run clean
```

This will generate `css/griddock.min.css` from the source file.

## 📦 What's Included

```
griddock/
├── css/
│   ├── griddock.css      # Development version
│   └── griddock.min.css  # Production version
├── demo.html             # Comprehensive demo
├── package.json
└── README.md
```

## 🔗 Component Reference

### Layout
- **Container**: Responsive centered container
- **Grid System**: 12-column CSS Grid system
- **Section**: Content sections with spacing
- **Hero**: Large banner sections

### Elements
- **Button**: Versatile button component
- **Form Controls**: Input, textarea, select, checkbox, radio
- **Table**: Clean data tables
- **Typography**: Headings, text utilities

### Components
- **Card**: Flexible content containers
- **Message**: Alert and notification boxes
- **Modal**: Overlay dialogs
- **Navigation**: Navbar, breadcrumb, tabs

### Utilities
- **Spacing**: Margin and padding utilities
- **Colors**: Text and background colors
- **Display**: Show/hide utilities
- **Text**: Alignment and weight utilities

## 🌟 CSS Grid Advantages

Unlike traditional flexbox-based frameworks, Griddock leverages CSS Grid's unique capabilities:

1. **Two-dimensional layouts**: Control both rows and columns simultaneously
2. **Subgrid support**: Better nested grid alignment (where supported)
3. **Grid areas**: Named grid areas for complex layouts
4. **Auto-placement**: Intelligent automatic item placement
5. **Gap control**: Built-in gap management without margin hacks

## 🔄 Migration from Other Frameworks

Griddock uses familiar class names similar to Bulma, making migration straightforward:

### From Bulma
- Most class names are identical (`button`, `is-primary`, `card`, etc.)
- Grid system uses similar concepts but with CSS Grid power
- Components maintain the same structure and modifiers

### From Bootstrap
- Replace `container-fluid` with `container is-fluid`
- Replace `row`/`col-*` with `grid`/`span-*`
- Button and utility classes have similar patterns

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

## 📄 License

BSD 3-Clause License

## 🚀 Demo

Check out the comprehensive demo at `demo.html` to see all components in action.

---

Built with ❤️ using CSS Grid technology
