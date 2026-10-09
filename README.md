# KEMTECH Website

## Files
- `index.html`: the supplied KEMTECH website HTML. The original HTML content is preserved.
- `assets/README.txt`: notes for any future local images, icons, or other assets.

## Important
The current HTML already contains its CSS (`<style>` blocks) and JavaScript (`<script>` blocks) inside `index.html`.
Therefore, separate `style.css` or `script.js` files are not required for this version. Do not add empty CSS/JS files or change the HTML references without a deliberate refactor and testing.

The HTML also loads some libraries/fonts from external CDNs. Those are not local files in this repository.

## GitHub upload
Upload `index.html`, `README.md`, `.gitignore`, and the `assets` folder to the repository root.
Keep `index.html` at the repository root for a typical Vercel static site.

## Vercel
For this plain static HTML setup, choose `Other` as Framework Preset. The project Root Directory should be the folder containing `index.html`. Do not add a build command unless the project is later converted to a build-based framework.

## Security reminder
Never commit Supabase secret/service-role keys, database passwords, or other server secrets into HTML or a public client-side JavaScript file. Client-visible publishable keys still require correct database RLS policies.
