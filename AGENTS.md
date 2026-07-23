# AGENTS.md — Academic Templates

## Repository Layout
- `Essay/` — Academic essay template (`main.tex`, `diazessay.cls`, `sample.bib`, `Figures/`)
- `Project/` — Course project template (`main.tex`, `titlepage.tex`, `packages.sty`, `styles.sty`, `content/`, `bibliography.bib`)
- `homework.tex` — Problem set template
- `article.tex` — General academic article template

## Building and Testing
```bash
# Essay compilation
cd Essay && pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex

# Project compilation
cd Project && pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex

# Single-file templates (no bibliography)
pdflatex homework.tex
pdflatex article.tex
```
The triple compilation pass resolves cross-references, citations, and the table of contents.

## General Guidance
- Requires a LaTeX distribution (TeX Live recommended).
- Keep preamble in `.sty` files for projects; use inline `\usepackage{}` for single-file templates.
- Bibliography entries in BibLaTeX format inside `.bib` files.
- Graphics belong in a `Figures/` subdirectory.
- Use `amsmath` and `amssymb` for mathematical notation.
- These templates are used for coursework at Università degli Studi di Perugia.

## Commit Messages
- Follow the [Chris Beams](http://chris.beams.io/posts/git-commit-style/) style.
- Every commit should answer: what changed and why.

## Review Checklist
- Template compiles without errors on a clean TeX Live install.
- All cross-references resolve correctly.
- Bibliography compiles without warnings.
- No hardcoded personal information in template files.
