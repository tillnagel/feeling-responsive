---
layout: page
title:  "Outer Space Satellite Database 1974-2015"
subheadline: Satelliten sind aus unserem täglichen Leben nicht mehr wegzudenken.
teaser: " Es ist unglaublich, dass wir überall Anwendungen benutzen, die direkt mit Satelliten in Verbindung stehen.
Das interaktive Plakat ermöglicht dem Betrachter einen zeitlichen Überblick der Satellitenanzahl, Art des Satelliten und Besitzer- und Auftraggeberland."


header: no
show_meta: false
categories:
    - projects
image:
    title: header.jpg
    caption: Outer Space
author: Antonia Josefa Gluschak
---



Am 10.02.2009 kam es im Erdorbit zu einem folgeschweren Zusammenstoß. Ein Kommunikationssatellit namens Iridium 33 kreuzte die Bahn des bereits ausgedienten Satelliten Kosmos 2251, sodass die wodurch mehr als 2200 Fragmente in der Umlaufbahn verteilt wurden. Die Recherche zu dieser Kollision führte dazu, dass ich mir nähere Informationen einholte und auf eine Datenbank namens „UCS Satellite Database“ gestoßen bin. Diese Datenbank ist von Experten der Union of Concerned Scientists (UCS) zusammengestellt worden. Die Liste enthält Informationen über mehr als 1000 operative Satelliten.

Die Grundlage der Visualisierung basiert auf drei Fragestellungen. Wie viele Satelliten besitzt jede individuelle Nation? Welche Länder kooperieren miteinander? Und in welchen Jahren gab es einen Satellitenaufschwung?



<div class="flex-video"><iframe src="https://player.vimeo.com/video/175610396" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe></div>



<figure>
  <img src="{{ site.urlimg }}/interaktiv2.jpg" />
  <figcaption >Übersicht der Screens</figcaption>
</figure>



## Prototypen

Meine interaktive Anwendung hat einen Startscreen. Der Startscreen wurde in Cinema 4D animiert und in Adobe After Effect farblich und typografisch bearbeitet.
Desweiteren wird ein radiales „Chord Diagramm“ angezeigt, was die Kooperationen zwischen verschiedenen Ländern darstellt. Je ausgeprägter die Linien, desto intensiver die Zusammenarbeit zwischen den Ländern. Mit der linken Maustaste kann ein Land ausgewählt werden.


<figure>
  <img src="{{ site.urlimg }}/radchorddiagramm.jpg" />
  <figcaption >Radiales Chord Diagramm. Es werden die Verbindungen zwischen Betreiberland und Auftraggeberland angezeigt.</figcaption>
</figure>



Das aus­gewählte Land wird in der Weltkarte oberhalb angezeigt.


<figure>
  <img src="{{ site.urlimg }}/kartenansicht.jpg" />
  <figcaption >Zur Übersicht, wird das ausgewählte Land in der Weltkarte angezeigt.</figcaption>
</figure>


 Im mittleren Liniendiagramm wird die Anzahl der Satelliten in Abhängigkeit von der Jahreszahl abgebildet. Ist kein Land gewählt, erscheinen globale Informationen.


<figure>
  <img src="{{ site.urlimg }}/diagramm.jpg" />
  <figcaption >Anzahl der Satellitenarten wird dargestellt.</figcaption>
</figure>
