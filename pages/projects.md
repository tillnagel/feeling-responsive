---
layout: page-fullwidth
title:  "Urbane Ebenen"
subheadline:  "Projektblog MM|VR Design 2016"
teaser: "Im Kurs wurden anhand aktueller Design- und Forschungsansätze der Datenvisualisierung neue Konzepte entwickelt, um Menschen einen visuellen und greifbaren Zugang zur Stadt zu geben. Diese Seite stellt die von den Studierenden gestalteten Projekte vor."
permalink: /projects/
header: no
---
*Urbane Ebenen* ist ein Kurs unter der Leitung von Gastprofessor Dr. [Till Nagel][1], mit Unterstützung von Mathias Jüsche.<br/>Sommersemester 2016,  Burg Giebichenstein Kunsthochschule Halle, am Studiengang [Multimedia|VR-Design][2].
<!--more-->

<div class="row t60">
    <div class="medium-4 columns b30">
      <a href="http://phlow.github.io/feeling-responsive/blog/">
        <img src="{{ site.urlimg }}/project-mathias.jpg" />
        <h2 class="font-size-h3 t10">Radial Tree Places</h2>
        <p>Lorem ipsum dolores sit amet.</p>
      </a>
    </div>
    <div class="medium-4 columns b30">
        <img src="{{ site.urlimg }}/project-sophiemel.jpg" />
        <h2 class="font-size-h3 t10">Wegbegleiter</h2>
        <p>Lorem ipsum dolores sit amet.</p>
    </div>
    <div class="medium-4 columns b30">
        <img src="{{ site.urlimg }}/project-marcel.jpg" />
        <h2 class="font-size-h3 t10">Neue Gefühle</h2>
        <p>Visueller Vergleich der Sentiments und Bilder von Nachrichtenseiten.</p>
    </div>
</div>


{% for post in site.categories.projects %}
{% assign rowfinder = forloop.index | modulo: 3 %}
{% if rowfinder == 1 %}
<div class="row">
{% endif %}
    <div class="medium-4 columns b30" style="float:left">
        <a href="{{ site.url }}{{ post.url }}">
        <img src="{{ site.urlimg }}/{{post.image.title}}" />
        <h2 class="font-size-h3 t10">{{ post.title }} ({{forloop.index}})</h2>
        <p>{{ post.subheadline }}</p>
        </a>
    </div>
{% if rowfinder == 0 %}
</div>
{% endif %}
{% endfor %}
{% if rowfinder != 0 %}
</div>
{% endif %}



[1]: http://www.tillnagel.com
[2]: http://www.burg-halle.de/design/multimediavr-design/
