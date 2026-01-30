# Mobile Responsiveness & Tailwind CSS

This project now uses Tailwind CSS to handle mobile responsiveness and modern layout utilities.

## Prerequisites

- Node.js (v14 or higher)
- npm

## Rebuilding CSS

If you make changes to PHP files or the `assets/css/tailwind-input.css` file, you need to regenerate the output CSS.

Run the following command in the root directory:

```bash
npm run build:css
```

This will update `assets/css/tailwind-output.css`.

## Development

For continuous watching of changes:

```bash
npx tailwindcss -i ./assets/css/tailwind-input.css -o ./assets/css/tailwind-output.css --watch
```

## Structure

- `tailwind.config.js`: Configuration for Tailwind, including paths to scan for class names.
- `assets/css/tailwind-input.css`: The source CSS file containing Tailwind directives and custom CSS if needed.
- `assets/css/tailwind-output.css`: The generated CSS file included in the application.
