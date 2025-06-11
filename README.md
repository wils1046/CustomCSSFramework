# Modern SCSS Framework

A modular, theme-based SCSS framework featuring a vibrant sunset color scheme with modern glassmorphism effects.

## Installation

### Prerequisites

- Sass/SCSS compiler (Dart Sass recommended)
- Modern web browser with CSS Grid and Flexbox support

### Setup

1. **Clone or download** the project files
2. **Install Sass** (if not already installed):
   ```bash
   npm install -g sass
   ```

3. **Compile the SCSS**:
   ```bash
   sass --watch src/main.scss css/style.css
   ```

4. **Link the compiled CSS** in your HTML:
   ```html
   <link rel="stylesheet" href="./css/style.css">
   ```

## Usage

### Basic HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Project</title>
    <link rel="stylesheet" href="main.css">
</head>
<body>
    <div class="container">
        <h1 class="text-primary mb-4">Hello World</h1>
        <p class="text-secondary">Start building with our SCSS framework!</p>
        <button class="btn btn-primary">Get Started</button>
    </div>
</body>
</html>
```

### Components

#### Buttons
```html
<button class="btn btn-primary">Primary Button</button>
<button class="btn btn-secondary">Secondary Button</button>
<button class="btn btn-success">Success Button</button>
<button class="btn btn-danger">Danger Button</button>
```

#### Cards
```html
<div class="card">
    <div class="card-header">
        <h4 class="m-0">Card Title</h4>
    </div>
    <div class="card-body">
        <p>Card content goes here...</p>
    </div>
</div>
```

#### Forms
```html
<div class="form-group">
    <label for="email" class="form-label">Email</label>
    <input type="email" id="email" class="form-control" placeholder="Enter email">
</div>
```

#### Tables
```html
<table class="table">
    <thead>
        <tr>
            <th>Name</th>
            <th>Email</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>John Doe</td>
            <td>john@example.com</td>
        </tr>
    </tbody>
</table>
```

#### Images
```html
<img src="image.jpg" alt="Description" class="img-fluid">
<img src="image.jpg" alt="Description" class="img-thumbnail">
<img src="image.jpg" alt="Description" class="img-rounded">
<img src="image.jpg" alt="Description" class="img-circle">
```

#### Lists
```html
<ul class="list-disc">
    <li>Bullet point item</li>
    <li>Another item</li>
</ul>

<ol class="list-decimal">
    <li>Numbered item</li>
    <li>Another numbered item</li>
</ol>

<ol class="list-lower-alpha">
    <li>Alpha item (a, b, c)</li>
    <li>Another alpha item</li>
</ol>
```

### Layout System

#### Container
```html
<div class="container">
    <!-- Your content here -->
</div>
```

#### Grid System
```html
<div class="grid">
    <div>Grid item 1</div>
    <div>Grid item 2</div>
    <div>Grid item 3</div>
</div>
```

### Utility Classes

#### Text Colors
```html
<p class="text-primary">Primary text color</p>
<p class="text-secondary">Secondary text color</p>
<p class="text-success">Success text color</p>
<p class="text-danger">Danger text color</p>
<p class="text-info">Info text color</p>
```

#### Background Colors
```html
<div class="bg-primary p-4">Primary background</div>
<div class="bg-secondary p-4">Secondary background</div>
```

#### Spacing
```html
<!-- Margins -->
<div class="mt-5 mb-8">Margin top 5, bottom 8</div>
<div class="mx-auto">Centered horizontally</div>

<!-- Padding -->
<div class="p-4">Padding 4 on all sides</div>
<div class="px-6 py-3">Horizontal padding 6, vertical padding 3</div>
```

#### Typography
```html
<p class="fs-xs">Extra small text</p>
<p class="fs-sm">Small text</p>
<p class="fs-base">Base text (default)</p>
<p class="fs-lg">Large text</p>
<p class="fs-xl">Extra large text</p>
```

## Customization

### Modifying Colors

Edit `src/variables/_colors.scss`:
```scss
// Replace with your preferred colors
$sunset-orange: #your-primary-color;
$ocean-teal: #your-secondary-color;
$golden-yellow: #your-info-color;
$coral-red: #your-danger-color;
$mint-green: #your-success-color;
$charcoal-black: #your-dark-color;
$cream-white: #your-light-color;
```

### Customizing Theme

Edit `src/variables/_theme.scss`:
```scss
$theme: (
    primary: colors.$your-primary,
    secondary: colors.$your-secondary,
    danger: colors.$your-danger,
    success: colors.$your-success,
    info: colors.$your-info,
    dark: colors.$your-dark,
    light: colors.$your-light
);
```

### Adding Custom Spacing

Edit `src/variables/_sizing.scss`:
```scss
$spacing: (
    0: 0,
    1: 0.25rem,
    2: 0.5rem,
    // Add your custom spacing values
    custom: 2.5rem,
    large: 4.5rem,
);
```

### Custom Typography

Edit `src/variables/_typography.scss`:
```scss
// Change font families
$font-family-heading: "Your Heading Font", sans-serif;
$font-family-body: "Your Body Font", sans-serif;

// Modify font sizes
$sizes: (
    xs: 0.75rem,
    sm: 0.875rem,
    base: 1rem,
    lg: 1.125rem,
    // Add custom sizes
    custom: 1.375rem,
);
```

### Custom Button Styles

Edit `src/base/_buttons.scss`:
```scss
// Add custom button variant
.btn-custom {
    background: linear-gradient(135deg, #your-color1 0%, #your-color2 100%);
    color: white;
}
```

### Custom Background Utilities

Edit `src/variables/_background.scss`:
```scss
// Add custom background
.bg-custom {
    background: linear-gradient(135deg, #your-color1 0%, #your-color2 100%) !important;
    color: white;
}
```

### Font Import Customization

Edit `src/base/_inter-source.scss`:
```scss
// Replace with your preferred fonts
@import url('https://fonts.googleapis.com/css2?family=Your+Font:wght@300;400;500;600;700&display=swap');
```

### Component Customization

To customize any component, edit the corresponding file in `src/base/`:
- `_buttons.scss` - Button styles
- `_forms.scss` - Form layouts
- `_input.scss` - Input field styles
- `_tables.scss` - Table styles
- `_images.scss` - Image utilities
- `_layout.scss` - Layout components and cards
- `_lists.scss` - List styles

### Creating New Utilities

Add new utility classes in the appropriate variable files:

```scss
// In src/variables/_typography.scss
.text-custom {
    color: #your-color !important;
}

// In src/variables/_sizing.scss
.m-custom {
    margin: 3.5rem !important;
}
```

After making any changes, recompile your SCSS:
```bash
sass --watch src/main.scss css/style.css
```