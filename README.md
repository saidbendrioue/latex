# Projet LaTeX Hello World

Projet LaTeX minimal qui produit une page PDF « Hello World ».

## Prérequis

- TeX Live (`pdflatex`)

Sur Debian/Ubuntu :

```bash
sudo apt-get update
sudo apt-get install -y texlive-latex-base texlive-lang-french
```

## Compilation

```bash
cd latex
pdflatex main.tex
```

Le fichier `main.pdf` est généré dans ce dossier.
