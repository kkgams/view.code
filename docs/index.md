---
title: view.code
status: reference
---

# view.code

The local Project edits the real repository `README.md`; saving changes that file. Change `data-source` in the layout to edit another Project-local document.

The local Project registers canonical View entries directly from `src/` and published dependencies pinned in `gams.json`. Host-owned `/core`, `/util`, `/widgets` APIs and theme styling are not bundled.

Run `make open` on macOS Apple Silicon to launch the real Host. Run `npm test` for repository checks. Preview docs with `make serve-docs DOCS_PORT=8081`, validate with `make validate-docs`, and build a portable site with `make docs`. GitHub Pages runs that build on every push to `release`. Unit tag-release policies are unchanged.
