---
title: "Wildfires in Peru: what the satellite could measure"
orden: 2
collection: portfolio_en
translation: /proyectos/incendios-peru/
date: 2026-10-22 12:00:00 -0500
permalink: /en/projects/peru-wildfires/
excerpt: "In Chichas (Arequipa), 1,690 ha burned in October 2026. Only 4 of the 20 largest fires could be measured: clouds covered the rest."
pregunta: "How much burned in Peru's largest fires in October 2026?"
resultado: "In Chichas (Arequipa), **1,690 ha** burned, **4.3%** of the district, in an area with no heat hotspot recorded between 2012 and 2025, which rules out recurring managed burning. Only **4 of the 20** largest fires could be measured; clouds covered the rest."
image: incendios-chichas.webp
image_alt: "Map of the burned area in Chichas (Arequipa) measured with Sentinel-2, with fire severity in colors and VIIRS heat hotspots as dots"
etiquetas: "Remote sensing · Sentinel-2 · NASA FIRMS"
destacado: true
categorias: [teledeteccion, datos-abiertos]
embed: https://gabriela-pozo.github.io/incendios-peru/
galeria:
  - src: incendios-chichas.webp
    label: "Chichas"
    alt: "Map of the burned area in Chichas (Arequipa) measured with Sentinel-2, with fire severity in colors and VIIRS heat hotspots as dots"
    caption: "Figure. Burned area in Chichas with Sentinel-2 (15 to 20 October 2026); dots are VIIRS heat hotspots. Sources: NASA FIRMS, Copernicus Sentinel-2 and ESA WorldCover 2021."
  - src: incendios-nacional.webp
    label: "The 20 fires"
    alt: "Map of Peru with 8,637 VIIRS heat hotspots between 14 and 21 October 2026; four measured fires marked in green and sixteen not measurable in gray"
    caption: "Figure. 8,637 VIIRS hotspots from 14 to 21 October 2026 and the 20 fires with the most hotspots: 4 measured and 16 not measurable. Sources: NASA FIRMS and GADM 4.1."
cifra: "1,690 ha"
cifra_pie: "burned in an area with no hotspots recorded between 2012 and 2025"
figcaption: "Figure. Burned area in Chichas with Sentinel-2 (15 to 20 October 2026); dots are VIIRS heat hotspots. Sources: NASA FIRMS, Copernicus Sentinel-2 and ESA WorldCover 2021."
repo: https://github.com/gabriela-pozo/incendios-peru
demo: https://gabriela-pozo.github.io/incendios-peru/
demo_label: "Page"
---

## Before and after

{% include compare.html antes="chichas-antes.webp" despues="chichas-despues.webp" etiqueta_antes="15 Oct 2026" etiqueta_despues="20 Oct 2026" alt_antes="True-color Sentinel-2 image of the Chichas area on 15 October 2026, before the fire" alt_despues="True-color Sentinel-2 image of the same area on 20 October 2026, with the dark scar of the fire" pie="Figure. True-color Sentinel-2, same crop and color adjustment. The white and dark patches at the lower right on 20 October are clouds and their shadows." id="cmp-chichas" %}

## Sources

The map combines heat hotspots from [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/) (VIIRS), [Copernicus Sentinel-2](https://planetarycomputer.microsoft.com/dataset/sentinel-2-l2a) imagery from Planetary Computer and the [ESA WorldCover 2021](https://esa-worldcover.org/) land cover. The figures come from the [repository](https://github.com/gabriela-pozo/incendios-peru) and the [project page](https://gabriela-pozo.github.io/incendios-peru/). The map does not replace official reports.
