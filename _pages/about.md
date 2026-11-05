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
  <p class="eyebrow">Economista · Datos abiertos del Perú</p>
  <h1 id="nombre" class="hero__name">Gabriela Pozo</h1>
  <p class="hero__tagline">Datos del Perú, con sus límites a la vista.</p>
  <p class="hero__bio">Bachiller en Economía con experiencia en seguimiento de indicadores y tableros en Power BI en CEPLAN y el MIMP. Hoy uso Python y datos abiertos para responder preguntas sobre el Perú, y cuento también lo que no se pudo medir.</p>
  <ul class="chips" aria-label="Herramientas y temas">
    <li>Python</li>
    <li>Power BI</li>
    <li>STATA</li>
    <li>Datos abiertos</li>
  </ul>
  <p class="hero__actions">
    <a class="btn" href="#proyectos">Ver proyectos</a>
    <a class="btn btn--outline" href="https://github.com/{{ site.author.github }}" rel="noopener"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
    {%- if site.author.linkedin %}
    <a class="btn btn--outline" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" rel="noopener"><i class="fa-brands fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
    {%- endif %}
    <a class="btn btn--outline" href="mailto:{{ site.author.email }}"><i class="fa-solid fa-envelope" aria-hidden="true"></i> Correo</a>
    {%- include cv-button.html -%}
  </p>
</section>

<section id="proyectos" class="section" aria-labelledby="t-proyectos">
  <h2 id="t-proyectos" class="section__title">Proyectos</h2>
  <p class="home-lead">Cinco preguntas sobre el Perú, respondidas con datos abiertos. Cada tarjeta muestra la pregunta, el resultado y la fuente; abre la vista interactiva para explorarla tú misma.</p>
  <div class="filters" role="group" aria-label="Filtrar proyectos por tipo" data-filters>
    <button type="button" data-filter="todos" aria-pressed="true">Todos</button>
    <button type="button" data-filter="dashboards" aria-pressed="false">Dashboards</button>
    <button type="button" data-filter="teledeteccion" aria-pressed="false">Teledetección</button>
    <button type="button" data-filter="ia" aria-pressed="false">IA</button>
    <button type="button" data-filter="datos-abiertos" aria-pressed="false">Datos abiertos</button>
  </div>
  <p class="filters__status" id="filters-status" role="status" aria-live="polite"></p>
  <div class="cards">
    {%- assign proyectos = site.portfolio | sort: "orden" -%}
    {%- for p in proyectos -%}
      {% include project-card.html proyecto=p destacado=forloop.first %}
    {%- endfor -%}
  </div>
</section>

<section id="cv" class="section" aria-labelledby="t-cv">
  <h2 id="t-cv" class="section__title">Experiencia</h2>
  <p class="home-lead">Prácticas preprofesionales en seguimiento de indicadores y tableros.</p>
  <p class="cv__download">{% include cv-button.html %}</p>
  <div class="cv-entry">
    <p class="cv-entry__head"><strong>CEPLAN</strong><span>2024-2025</span></p>
    <p class="cv-entry__body">Estudios prospectivos y tablero de control en Power BI.</p>
  </div>
  <div class="cv-entry">
    <p class="cv-entry__head"><strong>MIMP</strong><span>2023-2024</span></p>
    <p class="cv-entry__body">Seguimiento de indicadores de población.</p>
  </div>
  <div class="cv-entry">
    <p class="cv-entry__head"><strong>Gerencia Regional de Comercio Exterior, Turismo y Artesanía del Cusco</strong><span>2022</span></p>
    <p class="cv-entry__body">Indicadores de turismo.</p>
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
