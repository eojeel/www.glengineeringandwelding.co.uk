# css/tailwind.css

Pre-built, minified Tailwind CSS (replaces the runtime `@tailwindcss/browser` script for performance).
Rebuild after changing utility classes in `index.html`:

```
npm i --no-save tailwindcss@4 @tailwindcss/cli@4
printf '@import "tailwindcss";\n@source "../index.html";\n' > /tmp/in.css
npx @tailwindcss/cli -i /tmp/in.css -o css/tailwind.css --minify
```
