# Vora — Content Site

Static site for Vora content. No build step, no framework — plain HTML/CSS served by GitHub Pages.

## Structure

```
index.html          — Home page
blog/
  index.html        — Blog listing
  nyknym/
    index.html      — "Not Your Keys, Not Your Mind" presentation
assets/
  css/style.css     — Shared styles
  nyknym/           — Slide images for NYKNYM presentation
  img/              — Shared images
```

## Adding a new blog post

1. Create a folder under `blog/` with the post slug: `blog/my-post/`
2. Add an `index.html` inside it
3. Use the NYKNYM page as a template — copy it, change the content
4. Add images to `assets/my-post/` if needed
5. Update `blog/index.html` to add the post to the listing

## Local preview

Open any HTML file directly in a browser, or run a local server:

```
cd vora-site
python3 -m http.server 8000
```

Then visit `http://localhost:8000`

## Deployment

This repo is configured for GitHub Pages. Push to `main` and the site deploys automatically.

To connect a custom domain (e.g., vora.io), add the domain to the `CNAME` file and configure DNS.
