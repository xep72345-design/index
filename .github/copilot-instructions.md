<!-- .github/copilot-instructions.md -->
# Copilot instructions for this repository ✅

## Project snapshot
- Single-page static site: `index.html` (markup) + `style.css` (presentation).
- No build system, package manager, or tests detected. Changes are validated by opening the files in a browser.

## What the project is for (big picture)
- Minimal static demo / landing page. Keep changes focused and light-weight: small HTML/CSS edits, text updates, and simple styling.

## Helpful context for edits (do these first) 🔧
- Always confirm `index.html` and `style.css` remain linked: `index.html` uses `<link rel="stylesheet" href="style.css">`.
- Prefer making incremental, minimal changes (this is a micro repo). For styling, update `style.css`; avoid inlined styles unless necessary.

## How to run & preview changes (developer workflow) ⚡
- There is no build step. Preview by opening `index.html` in a browser.
- For a lightweight local server (recommended for relative assets), run:
  - Python: `python -m http.server 8000` in repo root, then open `http://localhost:8000`.
  - Node (if available): `npx serve .`

## Patterns & conventions to follow
- Keep structure flat (root files only). Add files to the repo root unless adding a clear directory (e.g., `assets/`, `images/`).
- Naming: use lowercase filenames without spaces (e.g., `style.css`, `index.html`).
- Keep CSS small and simple; prefer existing selectors (e.g., `h1 { color: blue; }`).

## Examples (explicit code references)
- Update heading text: edit `index.html`'s `<h1>this is index</h1>`.
- Change style: edit `style.css` to modify `h1` rules.

## Tests, CI, and build notes
- No tests or CI configured. If adding automation, include a `README.md` and a simple GitHub Actions workflow that validates HTML/CSS linting or a static-server smoke test.

## PR guidance & message suggestions 💬
- Keep PRs small and focused. Example PR title: `style: tweak h1 color and spacing`.
- In the PR body, include before/after screenshots or a URL to the local preview when relevant.

## Do not assume
- There are no JS frameworks, bundlers, or package.json here — do not add complex build tooling without a clear justification.

---
If anything above is unclear or you want examples expanded, tell me which part to clarify and I will iterate. 🔁
