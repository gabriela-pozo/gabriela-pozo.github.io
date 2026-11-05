---
title: "Análisis exploratorio con datos abiertos"
orden: 5
collection: portfolio
permalink: /proyectos/datos-abiertos/
excerpt: "Cuadernos de análisis con datos abiertos sobre crisis fiscal, consumo global de energía y pérdida de cobertura arbórea en el Perú."
pregunta: "¿Cómo ha evolucionado cada año la pérdida de cobertura arbórea en el Perú, según Global Forest Watch?"
resultado: "El pico de la serie 2001-2024 fue en 2017, con **303&nbsp;217 ha** de cobertura arbórea perdidas."
image: cobertura-arborea-peru.webp
image_alt: "Gráfico de barras de la pérdida anual de cobertura arbórea en el Perú entre 2001 y 2024, con 2017 resaltado como el año de mayor pérdida"
figcaption: "Figura. Pérdida anual de cobertura arbórea en el Perú, 2001-2024. Fuente: Global Forest Watch (UMD), umbral de cobertura de 30 %."
etiquetas: "Cuadernos · Datos abiertos · Global Forest Watch"
categorias: [datos-abiertos]
cifra: "303 217 ha"
cifra_pie: "de cobertura arbórea perdida en 2017, el máximo de la serie 2001-2024"
repo: https://github.com/gabriela-pozo/OurWorldData
demo: https://github.com/gabriela-pozo/OurWorldData/blob/main/notebooks/03_peru_tree_cover_loss.ipynb
demo_label: "Cuaderno"
---

## De dónde sale la cifra

El repositorio reúne tres análisis exploratorios con datos abiertos: crisis fiscal, consumo global de energía y pérdida de cobertura arbórea en el Perú.

La cifra de 2017 sale de la única celda de código del cuaderno [`03_peru_tree_cover_loss.ipynb`](https://github.com/gabriela-pozo/OurWorldData/blob/main/notebooks/03_peru_tree_cover_loss.ipynb), que consulta la API de [Global Forest Watch](https://www.globalforestwatch.org/) (conjunto `gadm__tcl__iso_change`, versión v20250515, umbral de cobertura de 30 %) e imprime la tabla `df_final`. En 2017 la tabla marca 303 216,79 ha.

El gráfico de arriba está hecho con los valores de esa misma salida.
