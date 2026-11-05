---
permalink: /
title: "Gabriela Pozo"
seo_title: "Gabriela Pozo · Datos abiertos sobre el Perú"
hide_title: true
redirect_from:
  - /about/
  - /about.html
  - /proyectos/
  - /cv/
  - /resume
---

<section id="inicio" class="hero" aria-labelledby="nombre">
  <h1 id="nombre" class="hero__name">Gabriela Pozo</h1>
  <p class="hero__tagline">Datos del Perú, con sus límites a la vista.</p>
  <p class="hero__bio">Trabajo con indicadores, metas y tableros de control para apoyar decisiones públicas: lo hice en CEPLAN y en el MIMP. Hoy uso datos abiertos para responder preguntas sobre el Perú, y cuento también lo que no se pudo medir.</p>
  <ul class="chips" aria-label="Áreas de trabajo">
    <li>Seguimiento de indicadores</li>
    <li>Estudios prospectivos</li>
    <li>Población y desarrollo</li>
    <li>Turismo</li>
    <li>Tableros de control</li>
    <li>Datos abiertos</li>
  </ul>
  <p class="tools-line">Herramientas: Python, Power BI, STATA.</p>
  <p class="hero__actions">
    <a class="btn" href="#proyectos">Ver proyectos</a>
    <a class="btn btn--outline" href="https://github.com/{{ site.author.github }}" rel="noopener"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
    {%- if site.author.linkedin %}
    <a class="btn btn--outline" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" rel="noopener"><i class="fa-brands fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
    {%- endif %}
    <a class="btn btn--outline" href="mailto:{{ site.author.email }}"><i class="fa-solid fa-envelope" aria-hidden="true"></i> Correo</a>
    {%- include cv-button.html -%}
  </p>

  <ul class="trail" aria-label="Experiencia en instituciones públicas">
    <li><strong>CEPLAN</strong><span>Estudios prospectivos, seguimiento de metas y tablero en Power BI</span></li>
    <li><strong>MIMP</strong><span>Seguimiento y validación de indicadores de población</span></li>
    <li><strong>Gerencia Regional de Comercio Exterior, Turismo y Artesanía del Cusco</strong><span>Informe de indicadores de turismo</span></li>
  </ul>
</section>

<section id="proyectos" class="section" aria-labelledby="t-proyectos">
  <h2 id="t-proyectos" class="section__title">Proyectos</h2>
  <p class="home-lead">Tres casos con imágenes y vista en vivo. Debajo, más trabajo con datos abiertos.</p>
  <div class="cards">
    {%- assign proyectos = site.portfolio | sort: "orden" -%}
    {%- for p in proyectos -%}
      {%- if p.destacado -%}
        {% include project-card.html proyecto=p destacado=forloop.first %}
      {%- endif -%}
    {%- endfor -%}
  </div>
  <h3 class="subhead">Más proyectos</h3>
  <div class="rows">
    {%- for p in proyectos -%}
      {%- unless p.destacado -%}
        {% include project-row.html proyecto=p %}
      {%- endunless -%}
    {%- endfor -%}
  </div>
</section>

<section id="actividad" class="section" aria-labelledby="t-actividad">
  <h2 id="t-actividad" class="section__title">Actividad en GitHub</h2>
  <p class="home-lead">Todo lo que ves aquí vive en repositorios públicos. Este es el calendario de mi actividad, tomado de <a href="https://github.com/{{ site.author.github }}" rel="noopener">mi perfil</a>.</p>
  <div class="activity" tabindex="0" role="group" aria-label="Calendario de contribuciones de GitHub (se desplaza horizontalmente)">
    <img src="https://ghchart.rshah.org/0A7466/{{ site.author.github }}" alt="Calendario de contribuciones de GitHub de {{ site.author.github }} durante el último año" width="720" height="112" loading="lazy" onerror="this.closest('section').hidden=true">
  </div>
</section>

<section id="contacto" class="section" aria-labelledby="t-contacto">
  <h2 id="t-contacto" class="section__title">Contacto</h2>
  <div class="contact">
    <p class="contact__text">¿Tienes una pregunta sobre el Perú que los datos puedan responder? Escríbeme y la conversamos.</p>
    <p class="contact__actions">
      <a class="btn" href="mailto:{{ site.author.email }}"><i class="fa-solid fa-envelope" aria-hidden="true"></i> {{ site.author.email }}</a>
      <a class="btn btn--outline" href="https://github.com/{{ site.author.github }}" rel="noopener"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
      {%- if site.author.linkedin %}
      <a class="btn btn--outline" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" rel="noopener"><i class="fa-brands fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
      {%- endif %}
    </p>
  </div>
</section>
