---
permalink: /
title: "Gabriela Pozo"
seo_title: "Gabriela Pozo · Datos abiertos sobre el Perú"
hide_title: true
redirect_from:
  - /about/
  - /about.html
---

<div class="home">
  <aside class="rail" aria-label="Perfil">
    <div class="rail__id">
      <img class="rail__photo" src="{{ '/images/foto.jpg' | prepend: site.baseurl }}" alt="Avatar de Gabriela Pozo, un patrón geométrico generado a partir de su usuario de GitHub" width="400" height="400" fetchpriority="high">
      <h1 id="nombre" class="rail__name">Gabriela Pozo</h1>
    </div>
    <p class="rail__tagline">Datos del Perú, con sus límites a la vista.</p>
    <p class="rail__bio">Bachiller en Economía con experiencia en seguimiento de indicadores y tableros en Power BI en CEPLAN y el MIMP. Hoy uso Python y datos abiertos para responder preguntas sobre el Perú, y cuento también lo que no se pudo medir.</p>
    <p class="rail__actions">
      <a class="btn btn--outline" href="https://github.com/{{ site.author.github }}" rel="noopener"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
      {%- if site.author.linkedin %}
      <a class="btn btn--outline" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" rel="noopener"><i class="fa-brands fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
      {%- endif %}
      <a class="btn btn--outline" href="mailto:{{ site.author.email }}"><i class="fa-solid fa-envelope" aria-hidden="true"></i> Correo</a>
      {%- include cv-button.html -%}
    </p>
  </aside>
  <section class="feed" aria-labelledby="destacados">
    <h2 id="destacados" class="feed__title">Proyectos destacados</h2>
    <p class="home-lead">Lo que une a mis proyectos: reglas escritas antes de mirar los datos, fuente enlazada en cada cifra y límites declarados.</p>
    <div class="cards">
      {%- assign proyectos = site.portfolio | sort: "orden" -%}
      {%- for p in proyectos limit: 3 -%}
        {% include project-card.html proyecto=p destacado=forloop.first %}
      {%- endfor -%}
    </div>
    <p class="home-more">Más proyectos: <a href="https://gabriela-pozo.github.io/Ficafe_2026/" rel="noopener">Archivo FICAFE</a></p>
  </section>
</div>
