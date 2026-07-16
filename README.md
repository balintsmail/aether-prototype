# Aether — Analyze Result v2 (prototype)

A static, self-contained build of the OPSWAT MetaDefender **Aether / Analyze Result v2**
UX prototype, hosted on GitHub Pages.

**Live:** https://GITHUB_USER.github.io/aether-prototype/

## About this build

- Client-side React SPA (BrowserRouter). All mock data is baked into the bundle — no backend.
- Trimmed to a single page (**Analyze Result v2**) with four tabs: **Overview, Similarity
  Search, IOC List, IOC Map**.
- Base path is `/aether-prototype/` to match the repository name (GitHub Pages project site).
- `404.html` is a copy of `index.html` so client-side deep links resolve (standard SPA-on-Pages
  fallback); `.nojekyll` disables Jekyll processing.

## Local preview

Because it is a client-side-routed SPA it must be served over HTTP (not opened via `file://`)
and from the `/aether-prototype/` base. Any static server with an SPA fallback works.

## Structure

```
index.html            app shell
404.html              SPA fallback (copy of index.html)
.nojekyll
vite.svg
assets/
  index-*.js          React bundle
  index-*.css         compiled CSS (all icons inlined as data URIs)
  *.woff2             Simplon Norm + Roboto fonts
```
