# AGENTS.md — LaTeX Academic Templates

## Project Overview
Ready-to-use LaTeX document templates for university coursework. Configured for computer science and engineering disciplines.

## Setup Commands
- Requires: TeX Live or MiKTeX distribution
- Compile essay: `cd Essay && pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex`
- Compile project: `cd Project && pdflatex main.tex && bibtex main && pdflatex main.tex`
- Triple compilation pass resolves cross-references, citations, and table of contents

## Template Structure
- `Essay/` — Academic essays with BibLaTeX bibliography (`main.tex`, `diazessay.cls`, `sample.bib`)
- `Project/` — Course projects with title page, packages, styles
- `homework.tex` — Problem sets with answer formatting
- `article.tex` — General-purpose academic article

## Code Style
- Use `\usepackage{}` in preamble, not scattered throughout
- Bibliography entries in BibLaTeX format
- Graphics in `Figures/` subdirectory
- Keep preamble clean — use `packages.sty` and `styles.sty` for project template

## Package Dependencies
- `amsmath`, `amssymb` — Math formatting
- `geometry` — Page layout
- `hyperref` — Clickable references
- `graphicx` — Image inclusion
- `biblatex` — Bibliography management
