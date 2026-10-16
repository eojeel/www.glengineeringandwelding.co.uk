# css/tailwind.css

Pre-built, minified Tailwind CSS (replaces the runtime `@tailwindcss/browser` script for performance).
Design tokens (brand colours, fonts) live in `css/input.css`. Rebuild after changing utility classes in `index.html`:

```
npm i --no-save tailwindcss@4 @tailwindcss/cli@4
npx @tailwindcss/cli -i css/input.css -o css/tailwind.css --minify
```
