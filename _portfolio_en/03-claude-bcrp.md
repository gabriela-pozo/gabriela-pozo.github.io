---
title: "Does Claude make up figures? Memory, web and the BCRP's MCP"
orden: 3
collection: portfolio_en
translation: /proyectos/claude-bcrp/
date: 2026-10-28 12:00:00 -0500
permalink: /en/projects/claude-bcrp/
excerpt: "With 10 questions and Claude Haiku, the MCP server got 10 right, the web 9 and memory 0."
pregunta: "Does Claude answer official BCRP data correctly depending on where it gets the information?"
resultado: "With 10 questions and Claude Haiku, the MCP server got **10** right, the web **9** and memory **0** (it said “I don't know”). When memory was denied the “I don't know” option, **7 of 10** answers came out wrong: 3 were real estimates and 4 a zero used as a placeholder."
image: claude-bcrp.webp
image_alt: "Stacked bar chart of Claude Haiku's correct answers, errors and “doesn't know” answers on 10 BCRP questions, depending on whether it uses memory, web or MCP"
etiquetas: "AI evaluation · MCP · BCRP"
destacado: true
categorias: [ia]
cifra: "10/10"
cifra_pie: "correct answers with the BCRP MCP server (web: 9, memory: 0)"
figcaption: "Figure. Correct answers, errors and “doesn't know” answers from Claude Haiku on 10 BCRP questions, depending on whether it uses memory, web or MCP."
repo: https://github.com/gabriela-pozo/mcp-bcrp
demo: https://github.com/gabriela-pozo/mcp-bcrp/blob/main/informe.md
demo_label: "Report"
---

## Results by query mode

<div class="bars" data-bars>
  <p class="bars__legend"><span class="bars__key bars__key--ok">Correct</span> <span class="bars__key bars__key--bad">Wrong</span> <span class="bars__key bars__key--na">Doesn't know</span></p>
  <ul class="bars__list">
    <li class="bars__row" tabindex="0" data-detail="Memory, base run: 10 of 10 answers were “I don't know”. No correct answers.">
      <span class="bars__name">Memory <small>base</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--na" style="flex:10">10</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="Memory, without the “I don't know” option: 7 of 10 answers were wrong and 3 were “doesn't know”. No correct answers.">
      <span class="bars__name">Memory <small>no null</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--bad" style="flex:7">7</span> <span class="bars__seg bars__seg--na" style="flex:3">3</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="Web, base run: 9 correct answers and 1 “doesn't know”.">
      <span class="bars__name">Web <small>base</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--ok" style="flex:9">9</span> <span class="bars__seg bars__seg--na" style="flex:1">1</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="BCRP MCP server, base run: 10 correct answers out of 10.">
      <span class="bars__name">MCP <small>base</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--ok" style="flex:10">10</span></span>
    </li>
    <li class="bars__row" tabindex="0" data-detail="BCRP MCP server, without the “I don't know” option: 10 correct answers out of 10.">
      <span class="bars__name">MCP <small>no null</small></span>
      <span class="bars__track"><span class="bars__seg bars__seg--ok" style="flex:10">10</span></span>
    </li>
  </ul>
  <p class="bars__detail" aria-live="polite">Hover over or focus a row to see its detail. “No null” takes away Claude's “I don't know” option.</p>
</div>

## Sources

The figures come from the project's [report](https://github.com/gabriela-pozo/mcp-bcrp/blob/main/informe.md) and [repository](https://github.com/gabriela-pozo/mcp-bcrp).
