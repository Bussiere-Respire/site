# Bussière Respire — GitHub Pages + Jekyll

Cette version utilise directement **Jekyll**, intégré à GitHub Pages. Il n'y a donc plus de `scripts/build.py`.

## Structure

- `_posts/` : articles Markdown des contributeurs
- `_layouts/` : HTML commun et modèle des articles
- `_config.yml` : configuration Jekyll
- `style.css` : design
- `comprendre/`, `quartier/`, `agir/`, `actualites/` : pages de section
- `images/` : images
- `.github/workflows/pages.yml` : publication GitHub Pages

## Ajouter un article

Créer `_posts/AAAA-MM-JJ-mon-article.md` :

```markdown
---
layout: article
title: "Mon article"
date: 2026-09-20
category: "Comprendre"
excerpt: "Une courte présentation."
---

# Mon article

Texte...

## Une sous-partie

Texte...
```

Le Markdown et le front matter sont traités directement par Jekyll.

## Publication

Un commit sur `main` lance le workflow GitHub Actions, construit le site avec Jekyll puis le publie sur GitHub Pages.

## Modifier le design

- HTML global : `_layouts/default.html`
- HTML des articles : `_layouts/article.html`
- CSS : `style.css`

Le code est volontairement explicite et commenté afin de faciliter les corrections et évolutions.
