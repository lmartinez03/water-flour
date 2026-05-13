# Water + Flour

Restaurant website for Water + Flour (formerly Ciccio & Tony's) in SoHo, Tampa.

## How it's built

Single-file static site. Everything lives in `Water_Flour.html` — HTML, all CSS in one big `<style>` block at the top, all JS in one `<script>` at the bottom. Images are under `images/` (and a few subfolders by section).

No build step, no framework, no dependencies. Open the file in a browser or serve the folder with any static file server.

## Local preview

```sh
# from this folder, pick any one:
python -m http.server 8000
# or
npx serve .
```

Then visit http://localhost:8000/Water_Flour.html

## Deploying to Vercel

This is a plain static site, so Vercel deploys it as-is — no framework preset needed. Connect this repo on vercel.com → New Project, accept the defaults. The default entry is `index.html`; if Vercel doesn't auto-redirect to `Water_Flour.html` you can either rename the file to `index.html` or add a `vercel.json` rewrite.
