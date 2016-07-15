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
    title: TourTracker/Tourtracker_Header.jpg
    caption: 2016 Version des TourTrackers
author: Alex Kaatz
---

Der TourTracker ist eine Anwendung für Fans, sich die Tourtermine ihrer Band anzeigen zu lassen. Diese werden nicht wie gewöhnlich einfach als Liste ausgegeben, sondern gleich als Punkte auf einer Karte angezeigt. Die Anwendung erleichtert das Auffinden von Konzerten in der Nähe. Konzerte werden nicht mehr in abstrakter Listenformsondern in Verbindung mit Kartendaten dargestellt. Die Punkte sind in chronologischer Reihenfolge verbunden und sind durch eine Farbkodierung in vergangene und noch austehende Auftritte unterscheidbar. Über den Kalender kann man sich Daten auf zwei verschiedene Arten eingrenzen lassen. In der ersten Ansicht, gleich nach dem Öffnen einer Tour, werden alle Daten angezeigt. Mit Klick auf einen Monat filtert der TourTracker alle Daten heraus, und es werden nurnoch Daten dieses Monats angezeigt.

## Visualization Design
*TourTracker 2016* beinhaltet die neuesten Tourdaten ausgewählter Bands visualisiert als Marker auf der Weltkarte. Mithilfe des Kalenders kann man sich spezielle Daten herausfiltern um die Ansicht einzugrenzen.

* Standartmäßig werden die aktuellen Daten der Tour von 2016 angezeigt. Man kann sich aber auch die Daten der vergangenen zwei Jahre angucken, um diese evtl. zu vergleichen.
* Zur Vereinfachung wird durch eine Farbkodierung die Tour unterschieden. Rot steht dabei für schon gespielte, gelb für noch ausstehende Termine.
* Durch den Kalender kann man sich auch nur die Daten eines Monats ausgeben lassen.

<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_VergleichKapellePetra.jpg" />
  <figcaption >Vergleich der Kapelle Petra Tour von 2015 und 2016</figcaption>
</figure>

<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_Kalender.jpg" />
  <figcaption >Standart Kalenderansicht und Auswähl des Monats August</figcaption>
</figure>


## Design Process
Mit der Anwendung wollte ich weg von den klassischen Ansichten von Tourdaten in Form von Listen. Eine reduzierte Karte erleichtert dabei dem Nutzer die Übersicht. Informationen zu den einzelnen Bands wurden von vorn herein nicht in den Prozess mit einbezogen, da ich das Augenmerk allein auf die Touren legen wollte. Der Kalender ist ein weiteres Werkzeug für den Nutzer die Daten einer Band weiter einzugrenzen. So werden zunächst alle Tourtermine auf der Karte und auch im Kalender angezeigt. Durch Auswahl eines Monats werden alle Termine ausserhalb des ausgewählten Monats ausgeblendet.

<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_RumjacksAugust.jpg" />
  <figcaption >Standart Kalenderansicht und Auswähl des Monats August</figcaption>
</figure>

## Daten
Um die einzelnen Lokations auf der Karte meiner Anwendung zu zeigen, habe ich die Daten der Seite *songkick.com* beziehen können. Die API lieferte neben dem Datum auch gleich gut auswertbare Angaben zu den einzelnen Lokations und Events, die ich in das Projekt mit einfließen lassen konnte.
