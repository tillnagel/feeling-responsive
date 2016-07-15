---
layout: page
title:  "TourTracker"
subheadline: Tourdaten auf einer Weltkarte darstellen
teaser: "Tourdaten einer Band tracken und anhand einer Weltkarte in chronologischer Reihenfolge darstellen."
header: no
show_meta: false
categories:
    - projects
image:
    title: cfcityflows-nyc.jpg
    caption: Citywide view showing bike trajectories
author: Alex Kaatz
---

Der TourTracker ist eine Anwendung für Fans, sich die Tourtermine ihrer Band anzeigen zu lassen. Diese werden nicht wie gewöhnlich einfach als Liste ausgegeben, sondern gleich als Punkte auf einer Karte angezeigt. Die Anwendung erleichtert das Auffinden von Konzerten in der Nähe. Konzerte werden nicht mehr in abstrakter Listenformsondern in Verbindung mit Kartendaten dargestellt. Die Punkte sind in chronologischer Reihenfolge verbunden und sind durch eine Farbkodierung in vergangene und noch austehende Auftritte unterscheidbar. Über den Kalender kann man sich Daten auf zwei verschiedene Arten eingrenzen lassen. In der ersten Ansicht, gleich nach dem Öffnen einer Tour, werden alle Daten angezeigt. Mit Klick auf einen Monat filtert der TourTracker alle Daten heraus, und es werden nurnoch Daten dieses Monats angezeigt. 

## Visualization Design
*cf. city flows* has three viewing modes, all visualizing trips of rented bikes, but focusing on different levels of spatial and temporal granularity of cycling mobility:

* The citywide view aggregates all trajectories of bike-sharing trips for a given day and animates the trails for trips at a given time.
* In the station view only the bike trips to and from a selected station are shown, allowing the distinction between incoming and outgoing.
* A small-multiple view visualizes spatiotemporal patterns for three selected stations each in an exploded view that separates incoming from outgoing and morning from afternoon/evening trips.

<figure>
  <img src="{{ site.urlimg }}/cf-view2-london-draft.jpg" />
  <figcaption >Eine Bildbeschreibung</figcaption>
</figure>


## Design Process
In our process of exploring the bike data, and designing the visualizations we created lots of visual experiments. Some of those we share below.


## Daten
