# Dreamscape Gardens CSS Style Guide

## Color Scheme and Typography

- **Colors:**

  - Primary (Blue): `#0077b6`
  - Secondary (Teal): `#0096c7`
  - Accent (Mint Green): `#48cae4`
  - Define these colors as CSS variables for easy maintenance and consistency.

- **Fonts:**
  - Primary Font: 'Raleway', sans-serif
  - Secondary Font: 'Montserrat', sans-serif
  - Use a consistent font stack and define it as a variable.

```css
:root {
  --primary-color: #0077b6;
  --secondary-color: #0096c7;
  --accent-color: #48cae4;
  --primary-font: "Raleway", sans-serif;
  --secondary-font: "Montserrat", sans-serif;
}
```

## General Principles

- **Consistency:** Ensure consistency across the CSS file.
- **Readability:** Prioritize readability with well-organized and formatted code.
- **Single File Management:** Since all CSS is in a single file, use comments to clearly separate sections.

## Formatting Rules

- **Indentation:** Use 2 spaces for indentation.
- **Brace Style:** Place opening braces on the same line as the selector and closing braces on a new line.
- **Selector and Declaration Separation:** Separate selectors and declarations by new lines.

## Naming Conventions

- **Class Names:** Use lowercase and hyphen-delimited (e.g., `.main-header`, `.nav-item`).
- **ID Names:** Use sparingly, following camelCase (e.g., `#mainContent`).
- **Descriptive Names:** Ensure names are clear and reflective of their function or style.

## CSS File Structure

- **Section Comments:** Use comments to define major sections, such as 'Header', 'Footer', 'Typography', 'Colors', etc.
- **Ordering:** Order properties logically (box model, positioning, typography) or alphabetically for consistency.

```css
/* Header Styles */
.header {
  ...;
}

/* Footer Styles */
.footer {
  ...;
}

/* Typography */
body {
  font-family: var(--primary-font);
}

h1,
h2,
h3 {
  font-family: var(--secondary-font);
}
```

## Responsive Design

- **Media Queries:** Place media queries near relevant rules. Aim for a mobile-first approach.

## Example

```css
/* Dreamscape Gardens Main Stylesheet */

/* Variables */
:root {
  --primary-color: #0077b6;
  --secondary-color: #0096c7;
  --accent-color: #48cae4;
  --primary-font: "Raleway", sans-serif;
  --secondary-font: "Montserrat", sans-serif;
}

/* Global Styles */
body {
  font-family: var(--primary-font);
  color: var(--primary-color);
}

/* Header Styles */
.header {
  background-color: var(--secondary-color);
  ...;
}

/* Navigation Styles */
.nav-item {
  font-family: var(--secondary-font);
  ...;
}

/* Media Queries */
@media (max-width: 768px) {
  .header {
    ...;
  }
}
```
