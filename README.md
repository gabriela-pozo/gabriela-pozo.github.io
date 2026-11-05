# Portafolio de Gabriela Pozo

Sitio personal publicado en https://gabriela-pozo.github.io

Bachiller en Economía. Uso Python y datos abiertos para responder preguntas sobre el Perú, y cuento también lo que no se pudo medir.

## Cómo está armado

- `_config.yml`: nombre, descripción, URL y datos de contacto.
- `_pages/about.md`: inicio (foto, bio, botones y proyectos destacados).
- `_portfolio/`: un archivo por proyecto. Los datos de la tarjeta (pregunta, resultado, imagen, enlaces) van en el encabezado del archivo.
- `_pages/cv.md`: CV breve.
- `_sass/custom/_gabriela.scss`: paleta, tipografía y componentes propios.
- `_ejemplos_sin_usar/`: contenido de ejemplo del template, fuera del sitio publicado.

## Pendientes antes de publicar

- Reemplazar `images/foto.jpg` (hoy es un marcador con las iniciales) por la foto real, con el mismo nombre.
- Subir `files/CV-Gabriela-Pozo.pdf` **sin teléfono ni dirección**. El botón "Descargar CV" aparece solo cuando el archivo existe.
- Completar `author.linkedin` en `_config.yml` (solo el usuario) para que aparezca el botón de LinkedIn.

## Publicación

Se publica sola con GitHub Actions al hacer push a `main` (Settings > Pages > Source: GitHub Actions).

## Créditos

Construido sobre la plantilla [Academic Pages](https://github.com/academicpages/academicpages.github.io) (licencia MIT, ver `LICENSE`), derivada de Minimal Mistakes.
