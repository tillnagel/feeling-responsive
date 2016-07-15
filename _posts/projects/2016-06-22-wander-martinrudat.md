---
layout: page
title:  "wander"
subheadline: A random generated route planner
teaser: “Not all those who wander are lost”
header: no
show_meta: false
categories:
    - projects
image:
    title: wander/teaser.png
    caption: Citywide view showing bike trajectories
author: Martin Rudat
---

“Not all those who wander are lost”

Dieses Zitat J.R.R Tolkiens hat mich dazu
inspiriert einen zufallsgenerierten Routenplaner zu konzipieren. Bei „wander“ soll es sich sich um eine Kombination aus mobiler App und Desktop Applikation handeln. Der Benutzer setzt einen Startpunkt und definiert die Entfernung, die er wandern will. Die App setzt einen Radius, entsprechend gesetzter Entfernung,  im Umkreis des Startpunktes und wählt einen Zufälligen Zielpunkt und Route aus. Der Benutzer soll dabei von einer magischen Melodie geleitet werden die am stärksten ist wenn der Benutzer die richtige Route einhält. Dabei wird die Richtung des Smartphones ausgewärtet, die die umliegende Umgebung zum Vorschein bringt.
(siehe Bild oben)
Ziel von „wander“ ist es, den Benutzer dazu anzuregen neue Orte seiner Umgebung kennenzulernen und seine Umgebung und deren Details besser wahrzunehmen. Er soll erkennen, dass nicht das unbekannte Ziel das Ziel ist sondern der Weg an sich.

## Visualization Design
*cf. city flows* has three viewing modes, all visualizing trips of rented bikes, but focusing on different levels of spatial and temporal granularity of cycling mobility:

* The citywide view aggregates all trajectories of bike-sharing trips for a given day and animates the trails for trips at a given time.
* In the station view only the bike trips to and from a selected station are shown, allowing the distinction between incoming and outgoing.
* A small-multiple view visualizes spatiotemporal patterns for three selected stations each in an exploded view that separates incoming from outgoing and morning from afternoon/evening trips.

<figure>
  <img src="{{ site.urlimg }}/indexical-vis.jpg" />
  <figcaption >Beispiel-Bild</figcaption>
</figure>



## Design Process
In our process of exploring the bike data, and designing the visualizations we created lots of visual experiments. Some of those we share below.


## Daten
