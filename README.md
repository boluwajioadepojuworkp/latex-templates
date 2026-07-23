# LaTeX Academic Templates

A collection of LaTeX document templates configured for university coursework in computer science and engineering disciplines. These templates handle formatting, bibliography management, and document structure so that the writer can focus exclusively on content.

## Templates

| Template | Entry Point | Application |
|----------|-------------|-------------|
| Essay | `Essay/main.tex` | Academic essays with BibLaTeX bibliography support |
| Project | `Project/main.tex` | Course projects with configurable title page, table of contents, and appendices |
| Homework | `homework.tex` | Problem sets and assignments with answer formatting |
| Article | `article.tex` | General-purpose academic article layout |

## Usage

```bash
cp -r Essay/ my-essay/
cd my-essay/
# Edit main.tex with your content
pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex
```

The triple compilation pass ensures that all cross-references, citations, and the table of contents are fully resolved.

## Requirements

- A LaTeX distribution (TeX Live recommended)
- BibLaTeX for bibliography processing
- Standard LaTeX packages: `amsmath`, `amssymb`, `geometry`, `hyperref`, `graphicx`

## License

MIT
