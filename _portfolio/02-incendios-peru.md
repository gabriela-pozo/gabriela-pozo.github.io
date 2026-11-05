---
title: "Incendios en el Perú: lo que el satélite alcanzó a medir"
orden: 2
collection: portfolio
date: 2026-10-22 12:00:00 -0500
permalink: /proyectos/incendios-peru/
excerpt: "En Chichas (Arequipa) ardieron 1 690 ha en octubre de 2026. Solo 4 de los 20 incendios más grandes se pudieron medir: las nubes taparon el resto."
pregunta: "¿Cuánto se quemó en los mayores incendios del Perú en octubre de 2026?"
resultado: "En Chichas (Arequipa) ardieron **1&nbsp;690 ha**, el **4,3&nbsp;%** del distrito, en una zona sin ningún foco registrado entre 2012 y 2025, lo que descarta una quema de manejo recurrente. Solo **4 de los 20** incendios más grandes se pudieron medir; las nubes taparon el resto."
image: incendios-chichas.webp
image_alt: "Mapa del área quemada en Chichas (Arequipa) medida con Sentinel-2, con la severidad del fuego en colores y los focos de calor VIIRS como puntos"
etiquetas: "Teledetección · Sentinel-2 · NASA FIRMS"
destacado: true
categorias: [teledeteccion, datos-abiertos]
embed: https://gabriela-pozo.github.io/incendios-peru/
galeria:
  - src: incendios-chichas.webp
    label: "Chichas"
    alt: "Mapa del área quemada en Chichas (Arequipa) medida con Sentinel-2, con la severidad del fuego en colores y los focos de calor VIIRS como puntos"
    caption: "Figura. Área quemada en Chichas con Sentinel-2 (15 al 20 de octubre de 2026); los puntos son focos de calor VIIRS. Fuentes: NASA FIRMS, Copernicus Sentinel-2 y ESA WorldCover 2021."
  - src: incendios-nacional.webp
    label: "Los 20 incendios"
    alt: "Mapa del Perú con 8 637 focos de calor VIIRS entre el 14 y el 21 de octubre de 2026; cuatro incendios medidos marcados en verde y dieciséis no medibles en gris"
    caption: "Figura. 8 637 focos VIIRS del 14 al 21 de octubre de 2026 y los 20 incendios con más focos: 4 medidos y 16 no medibles. Fuentes: NASA FIRMS y GADM 4.1."
cifra: "1 690 ha"
cifra_pie: "quemadas en una zona sin focos registrados entre 2012 y 2025"
figcaption: "Figura. Área quemada en Chichas con Sentinel-2 (15 al 20 de octubre de 2026); los puntos son focos de calor VIIRS. Fuentes: NASA FIRMS, Copernicus Sentinel-2 y ESA WorldCover 2021."
repo: https://github.com/gabriela-pozo/incendios-peru
demo: https://gabriela-pozo.github.io/incendios-peru/
demo_label: "Página"
---

## Antes y después

{% include compare.html antes="chichas-antes.webp" despues="chichas-despues.webp" etiqueta_antes="15 oct 2026" etiqueta_despues="20 oct 2026" alt_antes="Imagen Sentinel-2 en color real de la zona de Chichas el 15 de octubre de 2026, antes del incendio" alt_despues="Imagen Sentinel-2 en color real de la misma zona el 20 de octubre de 2026, con la cicatriz oscura del incendio" pie="Figura. Sentinel-2 en color real, mismo recorte y ajuste de color. Las manchas blancas y oscuras abajo a la derecha del 20 de octubre son nubes y sus sombras." id="cmp-chichas" %}

## Fuentes

El mapa combina focos de calor de [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/) (VIIRS), imágenes [Copernicus Sentinel-2](https://planetarycomputer.microsoft.com/dataset/sentinel-2-l2a) desde Planetary Computer y la cobertura de [ESA WorldCover 2021](https://esa-worldcover.org/). Las cifras salen del [repositorio](https://github.com/gabriela-pozo/incendios-peru) y de la [página del proyecto](https://gabriela-pozo.github.io/incendios-peru/). El mapa no reemplaza reportes oficiales.
