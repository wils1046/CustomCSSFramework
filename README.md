# CustomCSSFramework
# CustomCSSFramework
## ⚙️ Setup Instructions

This project uses Sass. Please compile `src/main.scss` to `css/main.css` before opening `index.html`:

```bash
sass --watch src/main.scss:css/main.css
⚠️ Note: The compiled main.css file is ignored in version control and not included in the repository. Each developer should generate it locally.

## 🎨 Color System

Our custom CSS framework includes a thoughtfully designed color system, defined using Sass variables for easy customization and scalability. The color palette includes:

- `$color-primary`: #2a9d8f – a calm, nature-inspired teal used for primary buttons and headings
- `$color-secondary`: #e9c46a – a warm yellow tone for accent elements
- `$color-accent`: #f4a261 – an energetic orange for highlights
- `$color-danger`: #e76f51 – a bold red tone for warnings or errors
- `$color-light`: #f1faee – soft background surfaces
- `$color-dark`: #264653 – deep blue for contrast or dark sections

Utility classes such as `.text-primary`, `.bg-accent`, and `.bg-dark` allow developers to easily apply the theme across elements. The system ensures visual consistency, accessibility, and ease of customization for any project.
