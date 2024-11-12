# LaTeX Academic Templates

**By Boluwaji Oluwaseyi Adepoju**

LaTeX templates for university essays, projects, homework, and articles. Built for the Programmazione e Gestione dei Sistemi Informatici (L-P03) degree at Università degli Studi di Perugia.

## Templates

| Template | File | Use For |
|----------|------|---------|
| Essay | `Essay/main.tex` | Academic essays with bibliography |
| Project | `Project/main.tex` | Course projects with title page |
| Homework | `homework.tex` | Problem sets and assignments |
| Article | `article.tex` | Generic academic article |

## Usage

```bash
cp -r Essay/ my-essay/
cd my-essay/
# Edit main.tex with your content
pdflatex main.tex && bibtex main && pdflatex main.tex
```

## License

MIT — Free to use, modify, and share.
