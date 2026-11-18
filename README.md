# CV LaTeX

Sources du CV :

- `resume.tex` — version mise en page (colonne marine)
- `resume-ats.tex` — version une colonne pour les formulaires en ligne
- `dossier.tex` — dossier de compétences (couverture navy/or, frise formations, expériences 2 colonnes)

## Compilation locale

XeLaTeX. `resume.tex` a besoin de deux passes.

```bash
xelatex resume.tex && xelatex resume.tex
xelatex resume-ats.tex
xelatex dossier.tex
```

## GitHub Actions

Chaque push sur `main` compile `resume.pdf`, `resume-ats.pdf` et `dossier.pdf`, les publie en artefacts du workflow, puis les enregistre dans le dépôt s'ils ont changé.
