# Repository Guidelines

## Project Overview
This repository is a marketing playbook + proof library with a GitHub Pages “decision dashboard”. The public-facing UI must stay action-first and one-screen; deep research lives in Markdown files.

## Project Structure
- `docs/` — GitHub Pages site (static HTML/CSS). This is the “decision filter” front.
- `docs/DECISION_FILTER.md` — source text for decision cards (keep short, decision-framed).
- `MARKETER_RESULT.md` — single source of truth for conclusions used on Pages.
- `DOCS/` — long-form writeups and supporting materials (including `.pdf`/`.docx`).
- `CASE_STUDIES/` — case notes (wins/failures).
- `RESOURCES/` — data files (`.csv`, `.json`), glossary, quote bank, tooling lists.
- `vibe-coding-app/` — experimental app/prototype work (keep isolated).

## Local Preview (No Build Step)
Pages is static; no bundler is required.
- Preview `docs/` locally: `python3 -m http.server -d docs 8080`
- Open: `http://localhost:8080`

## Content & UI Rules (Decision Dashboard)
- Pages must remain one screen (avoid scrolling on common laptop viewports).
- No articles, no long paragraphs, no navigation menus.
- Cards must be clear DO / DON’T / TEST decisions; keep lines short and scannable.
- Update `docs/index.html` only using conclusions present in `MARKETER_RESULT.md`.
- Keep exactly one “proof” entry point (button/link) to GitHub/`MARKETER_RESULT.md`.

## Style & Naming
- Markdown: headings + short blocks; prefer filenames like `START_RESTAURANT.md`.
- HTML/CSS: keep minimal, readable, and consistent; avoid heavy JS and animations.
- Data files: `RESOURCES/*.json` should be stable-key JSON, 2-space indentation.

## Commits & Pull Requests
- Commit messages follow an imperative, concise style: `Add ...`, `Docs: ...`, `Rebuild ...`.
- PRs: include a 1–2 sentence summary + a screenshot of the Pages single-screen view.
- Avoid directory-wide renames or restructuring unless the task requires it.

