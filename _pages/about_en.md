---
permalink: /en/
lang: en
translation: /
title: "Gabriela Pozo"
seo_title: "Gabriela Pozo · Open data analysis"
description: "Open-data analysis: the question, the finding with its source, and what could not be measured."
hide_title: true
---

<section id="inicio" class="hero" aria-labelledby="nombre">
  <div class="hero__head">
    {%- include foto.html -%}
    <div>
      <h1 id="nombre" class="hero__name">Gabriela Pozo</h1>
      <p class="hero__tagline">What the data says, and what it doesn't yet.</p>
    </div>
  </div>
  <p class="hero__bio">Open-data analysis: each case starts with a question, shows the finding with its source, and says what could not be measured. I come from tracking indicators in the public sector.</p>
  <ul class="chips" aria-label="Topics covered here">
    <li>Education</li>
    <li>Wildfires</li>
    <li>AI and official data</li>
    <li>Specialty coffee</li>
    <li>Tree cover</li>
  </ul>
  <p class="hero__actions">
    <a class="btn" href="#proyectos">Read the projects</a>
    <a class="btn btn--outline" href="https://github.com/{{ site.author.github }}" rel="noopener"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
    {%- if site.author.linkedin %}
    <a class="btn btn--outline" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" rel="noopener"><i class="fa-brands fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
    {%- endif %}
    <a class="btn btn--outline" href="mailto:{{ site.author.email }}"><i class="fa-solid fa-envelope" aria-hidden="true"></i> Email</a>
    {%- include cv-button.html -%}
  </p>
</section>

<section id="proyectos" class="section" aria-labelledby="t-proyectos">
  <h2 id="t-proyectos" class="section__title">Projects</h2>
  <p class="home-lead">Open-data cases. Each one poses a question, presents the finding and puts the source one click away.</p>
  <div class="cards">
    {%- assign proyectos = site.portfolio_en | sort: "orden" -%}
    {%- for p in proyectos -%}
      {%- if p.destacado -%}
        {% include project-card.html proyecto=p destacado=forloop.first %}
      {%- endif -%}
    {%- endfor -%}
  </div>
  <h3 class="subhead">More cases</h3>
  <div class="rows">
    {%- for p in proyectos -%}
      {%- unless p.destacado -%}
        {% include project-row.html proyecto=p %}
      {%- endunless -%}
    {%- endfor -%}
  </div>
</section>

<section id="contacto" class="section" aria-labelledby="t-contacto">
  <h2 id="t-contacto" class="section__title">Contact</h2>
  <div class="contact">
    <p class="contact__text">Do you have a question that data could answer? Write to me and let's talk.</p>
    <p class="contact__actions">
      <a class="btn" href="mailto:{{ site.author.email }}"><i class="fa-solid fa-envelope" aria-hidden="true"></i> {{ site.author.email }}</a>
      <a class="btn btn--outline" href="https://github.com/{{ site.author.github }}" rel="noopener"><i class="fa-brands fa-github" aria-hidden="true"></i> GitHub</a>
      {%- if site.author.linkedin %}
      <a class="btn btn--outline" href="https://www.linkedin.com/in/{{ site.author.linkedin }}" rel="noopener"><i class="fa-brands fa-linkedin" aria-hidden="true"></i> LinkedIn</a>
      {%- endif %}
    </p>
  </div>
</section>
