---
title: "Exploratory analysis with open data"
orden: 5
collection: portfolio_en
translation: /proyectos/datos-abiertos/
date: 2026-03-10 12:00:00 -0500
permalink: /en/projects/open-data/
excerpt: "Analysis notebooks with open data on the fiscal crisis, global energy consumption and tree cover loss in Peru."
pregunta: "How has tree cover loss in Peru changed year by year, according to Global Forest Watch?"
resultado: "The peak of the 2001-2024 series was in 2017, with **303,217 ha** of tree cover lost."
image: cobertura-arborea-peru.webp
image_alt: "Bar chart of annual tree cover loss in Peru between 2001 and 2024, with 2017 highlighted as the year with the greatest loss"
figcaption: "Figure. Annual tree cover loss in Peru, 2001-2024. Source: Global Forest Watch (UMD), 30% canopy cover threshold."
etiquetas: "Notebooks · Open data · Global Forest Watch"
categorias: [datos-abiertos]
cifra: "303,217 ha"
cifra_pie: "of tree cover lost in 2017, the maximum of the 2001-2024 series"
repo: https://github.com/gabriela-pozo/OurWorldData
demo: https://github.com/gabriela-pozo/OurWorldData/blob/main/notebooks/03_peru_tree_cover_loss.ipynb
demo_label: "Notebook"
---

## Where the figure comes from

The repository brings together three exploratory analyses with open data: the fiscal crisis, global energy consumption and tree cover loss in Peru.

The 2017 figure comes from the only code cell of the notebook [`03_peru_tree_cover_loss.ipynb`](https://github.com/gabriela-pozo/OurWorldData/blob/main/notebooks/03_peru_tree_cover_loss.ipynb), which queries the [Global Forest Watch](https://www.globalforestwatch.org/) API (dataset `gadm__tcl__iso_change`, version v20250515, 30% canopy cover threshold) and prints the `df_final` table. For 2017 the table shows 303,216.79 ha.

The chart above is made with the values from that same output.
