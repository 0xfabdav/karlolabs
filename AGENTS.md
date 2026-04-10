# Agent Notes

## Repo shape
- This is a plain static site: no package manager, build step, test suite, or CI config is present.
- Runtime entrypoint is `index.html`, which loads `styles.css` and assets from `public/`.

## Working rules for edits
- Keep asset paths relative to repo root (current HTML uses `public/logoK.png`).
- Preserve the single-page static setup (no JS framework/tooling assumptions).
- Maintain mobile behavior already implemented in `styles.css` (`@media (max-width: 640px)`).

## Verify changes
- Run a local static server from repo root: `python3 -m http.server 8000`.
- Open `http://localhost:8000` and check desktop + mobile widths.
