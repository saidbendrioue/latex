# CV LaTeX

Sources du CV. `resume.tex` est la version mise en page. `resume-ats.tex` est la version une colonne pour les formulaires en ligne.

## Compilation locale

XeLaTeX. `resume.tex` a besoin de deux passes.

```bash
xelatex resume.tex && xelatex resume.tex
xelatex resume-ats.tex
```

## GitHub Actions

Chaque push sur `main` compile `resume.pdf` et `resume-ats.pdf`, les publie en artefacts du workflow, puis les enregistre dans le dépôt s'ils ont changé.
