---
permalink: /
title: "Gabriela Pozo"
seo_title: "Gabriela Pozo · Análisis con datos abiertos"
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
  <p class="hero__tagline">Lo que dicen los datos, y lo que todavía no.</p>
  <p class="hero__bio">Análisis con datos abiertos. Cada publicación parte de una pregunta, muestra el hallazgo con su fuente y cuenta también lo que no se pudo medir. Vengo del seguimiento de indicadores y tableros en el sector público.</p>
  <ul class="chips" aria-label="Temas que se tratan aquí">
    <li>Educación</li>
    <li>Incendios forestales</li>
    <li>IA y datos oficiales</li>
    <li>Café especial</li>
    <li>Cobertura arbórea</li>
  </ul>
  <p class="hero__actions">
    <a class="btn" href="#proyectos">Leer los proyectos</a>
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
  <p class="home-lead">Casos con datos abiertos. Cada uno plantea una pregunta, expone el hallazgo y deja la fuente a un clic.</p>
  <div class="cards">
    {%- assign proyectos = site.portfolio | sort: "orden" -%}
    {%- for p in proyectos -%}
      {%- if p.destacado -%}
        {% include project-card.html proyecto=p destacado=forloop.first %}
      {%- endif -%}
    {%- endfor -%}
  </div>
  <h3 class="subhead">Más casos</h3>
  <div class="rows">
    {%- for p in proyectos -%}
      {%- unless p.destacado -%}
        {% include project-row.html proyecto=p %}
      {%- endunless -%}
    {%- endfor -%}
  </div>
</section>

<section id="contacto" class="section" aria-labelledby="t-contacto">
  <h2 id="t-contacto" class="section__title">Contacto</h2>
  <div class="contact">
    <p class="contact__text">¿Tienes una pregunta que los datos puedan responder? Escríbeme y la conversamos.</p>
    <p class="contact__actions">
      <a class="btn" href="mailto:{{ site.author.email }}"><i class="fa-solid fa-envelope" aria-hidden="true"></i> {{ site.author.email }}</a>
      <a class="btn btn--outline" href="https://github.com/{{ site.author.github }}" rel="noopener"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
      {%- if site.author.linkedin %}
      <a class="btn btn--outline" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" rel="noopener"><i class="fa-brands fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
      {%- endif %}
    </p>
  </div>
</section>
