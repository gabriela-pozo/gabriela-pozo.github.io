---
title: "¿Inventa cifras Claude? Memoria, web y MCP del BCRP"
orden: 3
collection: portfolio
date: 2026-10-28 12:00:00 -0500
permalink: /proyectos/claude-bcrp/
excerpt: "Con 10 preguntas y Claude Haiku, el servidor MCP acertó 10, la web 9 y la memoria 0."
pregunta: "¿Responde bien Claude a datos oficiales del BCRP según de dónde saque la información?"
resultado: "Con 10 preguntas y Claude Haiku, el servidor MCP acertó **10**, la web **9** y la memoria **0** (decía «no sé»). Al quitarle a la memoria la salida «no sé», **7 de 10** respuestas salieron mal: 3 eran estimaciones reales y 4 un cero usado como marcador."
image: claude-bcrp.webp
image_alt: "Gráfico de barras apiladas con aciertos, errores y respuestas «no sabe» de Claude Haiku en 10 preguntas del BCRP, según use memoria, web o MCP"
etiquetas: "Evaluación de IA · MCP · BCRP"
destacado: true
categorias: [ia]
cifra: "10/10"
cifra_pie: "respuestas correctas con el servidor MCP del BCRP (web: 9, memoria: 0)"
figcaption: "Figura. Aciertos, errores y respuestas «no sabe» de Claude Haiku en 10 preguntas del BCRP, según use memoria, web o MCP."
repo: https://github.com/gabriela-pozo/mcp-bcrp
demo: https://github.com/gabriela-pozo/mcp-bcrp/blob/main/informe.md
demo_label: "Informe"
---

## Resultados por modo de consulta

<div class="bars" data-bars>
  <p class="bars__legend"><span class="bars__key bars__key--ok">Acierta</span><span class="bars__key bars__key--bad">Se equivoca</span><span class="bars__key bars__key--na">No sabe</span></p>
  <ul class="bars__list">
    <li class="bars__row" tabindex="0" data-detail="Memoria, corrida base: 10 de 10 respuestas fueron «no sé». Ningún acierto.">
      <span class="bars__name">Memoria <small>base</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--na" style="flex:10">10</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="Memoria, sin la salida «no sé»: 7 de 10 respuestas salieron mal y 3 fueron «no sabe». Ningún acierto.">
      <span class="bars__name">Memoria <small>sin null</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--bad" style="flex:7">7</span><span class="bars__seg bars__seg--na" style="flex:3">3</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="Web, corrida base: 9 aciertos y 1 «no sabe».">
      <span class="bars__name">Web <small>base</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--ok" style="flex:9">9</span><span class="bars__seg bars__seg--na" style="flex:1">1</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="Servidor MCP del BCRP, corrida base: 10 aciertos de 10.">
      <span class="bars__name">MCP <small>base</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--ok" style="flex:10">10</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="Servidor MCP del BCRP, sin la salida «no sé»: 10 aciertos de 10.">
      <span class="bars__name">MCP <small>sin null</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--ok" style="flex:10">10</span></span>
    </li>
  </ul>
  <p class="bars__detail" aria-live="polite">Pasa el cursor o enfoca una fila para ver su detalle. «Sin null» quita a Claude la salida «no sé».</p>
</div>

## Fuentes

Las cifras salen del [informe](https://github.com/gabriela-pozo/mcp-bcrp/blob/main/informe.md) y del [repositorio](https://github.com/gabriela-pozo/mcp-bcrp) del proyecto.
