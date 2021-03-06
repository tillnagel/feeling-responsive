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
    caption:
author: Antonia Josefa Gluschak
---



Am 10.02.2009 kam es im Erdorbit zu einem folgeschweren Zusammenstoß. Ein Kommunikationssatellit namens Iridium 33 kreuzte die Bahn des bereits ausgedienten Satelliten Kosmos 2251, sodass die wodurch mehr als 2200 Fragmente in der Umlaufbahn verteilt wurden. Die Recherche zu dieser Kollision führte dazu, dass ich mir nähere Informationen einholte und auf eine Datenbank namens „UCS Satellite Database“ gestoßen bin. Diese Datenbank ist von Experten der Union of Concerned Scientists (UCS) zusammengestellt worden. Die Liste enthält Informationen über mehr als 1000 operative Satelliten.

Die Grundlage der Visualisierung basiert auf drei Fragestellungen. Wie viele Satelliten besitzt jede individuelle Nation? Welche Länder kooperieren miteinander? Und in welchen Jahren gab es einen Satellitenaufschwung?

<br/>
<figure>
  <img src="{{ site.urlimg }}/interaktiv2.jpg" />
  <figcaption >Übersicht der Screens</figcaption>
</figure>
<br/>
<div class="flex-video"><iframe src="https://player.vimeo.com/video/175610396" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe></div>
<br/>

<figure>
  <img src="{{ site.urlimg }}/UCS.jpg" />
  <figcaption >Datenbank von der UCS</figcaption>
</figure>



## Prototypen
Meine interaktive Anwendung hat einen Startscreen. Der Startscreen wurde in Cinema 4D animiert und in Adobe After Effect farblich und typografisch bearbeitet.
Desweiteren wird ein radiales „Chord Diagramm“ angezeigt, was die Kooperationen zwischen verschiedenen Ländern darstellt. Je ausgeprägter die Linien, desto intensiver die Zusammenarbeit zwischen den Ländern. Mit der linken Maustaste kann ein Land ausgewählt werden. Das aus­gewählte Land wird in der Weltkarte oberhalb angezeigt. Im mittleren Liniendiagramm wird die Anzahl der Satelliten in Abhängigkeit von der Jahreszahl abgebildet. Ist kein Land gewählt, erscheinen globale Informationen.


<figure>
  <img src="{{ site.urlimg }}/Cchart.jpg" />
  <figcaption > Gesamtüberblick der Kooperationen </figcaption>
</figure>

<figure>
  <img src="{{ site.urlimg }}/radchorddiagramm.jpg" />
  <figcaption >Radiales Chord Diagramm</figcaption>
</figure>

<figure>
  <img src="{{ site.urlimg }}/kartenansicht.jpg" />
  <figcaption >Weltkarte</figcaption>
</figure>

<figure>
  <img src="{{ site.urlimg }}/DiagrammAll.jpg" />
  <figcaption >Gesamtanzahl der Satellitenarten </figcaption>
</figure>

<figure>
  <img src="{{ site.urlimg }}/diagramm.jpg" />
  <figcaption >globale Informationen</figcaption>
</figure>


## Umsetzung

* Programmierung in Processing
* Cinema 4D Animation des Startbildschirm
* Farbkorrektur der Animation wurde in Adobe After Effect umgesetzt
