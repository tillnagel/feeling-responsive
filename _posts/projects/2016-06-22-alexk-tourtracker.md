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

Jeder kennt das: man streift mal wieder durch die Webseiten seiner Lieblingsbands um nach aktuellen Daten ihrer Tour zu suchen. Das erste was man dabei findet sind mal mehr, mal weniger lange Listen mit Namen von Städten die einem mal mehr, mal weniger bekannt sind. Der nächste Schritt ist dann meist noch über diverse Anbieter zu gucken, wo die einzelnen Städte liegen, und ob sich nicht doch der eine oder ander unbekannter Name im näherem Umfeld liegt. Um dieses Problem zu beheben, kam mir der Gedanke beides in einer Anwendung zu vereinen. So entstand der TourTracker. Dieser ist eine Anwendung für Fans und Supporter, sich die Tourtermine ihrer Bands anzeigen zu lassen. Jeder Termin wird gleich als Wegpunkt auf einer Karte angezeigt. Die Anwendung erleichtert somit das Auffinden von Konzerten in der Nähe. Die Punkte sind in chronologischer Reihenfolge verbunden und dabei durch eine Farbkodierung in vergangene und noch austehende Auftritte unterscheidbar. Über den Kalender kann man sich Daten auf zwei verschiedene Arten eingrenzen lassen. In der ersten Ansicht, gleich nach dem Öffnen einer Tour, werden alle Daten angezeigt. Mit Klick auf einen Monat filtert der TourTracker alle Daten heraus, und es werden nurnoch Daten dieses Monats angezeigt.

## Visualization Design

*TourTracker 2016* beinhaltet die neuesten Tourdaten ausgewählter Bands visualisiert als Marker auf der Weltkarte. Mithilfe des Kalenders kann man sich spezielle Daten herausfiltern um die Ansicht einzugrenzen.

* Standartmäßig werden die aktuellen Daten der Tour von 2016 angezeigt. Man kann sich aber auch die Daten der vergangenen zwei Jahre angucken, um diese evtl. zu vergleichen.
* Zur Vereinfachung wird durch eine Farbkodierung die Tour unterschieden. Rot steht dabei für schon gespielte, gelb für noch ausstehende Termine.
* Durch den Kalender kann man sich auch nur die Daten eines Monats ausgeben lassen.


<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_VergleichKapellePetra.jpg" />
  <figcaption >Vergleich der Kapelle Petra Tour von 2015 und 2016</figcaption>
</figure>

## Design Process

Am Anfang stand das geografische Problem, dass ich mich zwar in einem bestimmten Umkreis meines Wohnortes auskenne, aber darüber hinaus immer einen Mapanbieter zur Hilfe ziehen muss, wenn es um Locations meiner Lieblingsbands geht. Also wollte ich weg von den klassischen Ansichten von Tourdaten in Form von Listen und hin zu einer Überschaubaren Mapanwendung mit der ich diese visualisieren kann. Ich habe mich für eine sehr reduzierte Karte entschieden um unnötige geografische Informationen von vorn herein auszuklammern. Auch verzichtet die Anwendung auf weitere Informationen zu den einzelnen Bands, da ich direkt schon Fans und Supporter anspreche, die sich mit den Bands schon auskennen. Über einen Link kann man aber die Homepage der ausgewählten Band erreichen. In der Anwendung werden aktuelle und die Daten der letzen zwei Jahren visualisiert. Über eine Auswahl kann man sich die einzelnen Jahre mühelos anzeigen lassen. Ein weiteres Werkzeug für den Nutzer um Daten einer Band weiter einzugrenzen ist der Kalender.

<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_Kalender.jpg" />
  <figcaption >Standart Kalenderansicht und Auswähl des Monats August</figcaption>
</figure>

## Der Kalender

Der Kalender ist ein zentrales Werkzeug des Tourtrackers. Über den Kalender hat der Nutzer die Möglichkeit einen Zeitraum anzugeben, aus dem die Wegpunkte auf der Karte generiert werden. Nachdem der Nutzer entschieden hat welches Jahr er sich anzeigen lassen möchte, werden zunächst alle Daten des Jahres als Wegpunkte angezeigt. Dies kann jeh nach Dauer der Tour und Anzahl der Auftritte auch schon mal Unübersichtlich werden. Die erste Filtermöglichkeit ist hierfür ein *klick* auf einen Monat, den man sich anzeigen lassen will. Wenn man zum Beispiel weiß, das man im August frei hat, kann man diesen anklicken und es werden nur Daten aus diesem Monat angezeigt. Man kann aber auch weitere Monate dazuwählen, das Prinzip bei den Daten bleibt das selbe.
Der Nutzer kann aber auch zu einer andern Ansicht der Kalenders wechseln, um sich seine Zeitspanne individuell und auch über einen Monatswechsel hinaus anzeigen zu lassen. In der zweiten Kalenderansicht hat der Nutzer einen Slider mit dem er Anfang und auch Ende seiner Zeitspanne definieren kann. Diese Ansicht bietet sich an, weiß man das man zum Beispiel vom 26.4. bis 08.5. im Urlaub oder dienstlich unterwegs ist und nebenbei ein bisschen Zeit hat.

<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_Kalender_02.jpg" />
  <figcaption >Standart Kalenderansicht und Auswähl des Monats August</figcaption>
</figure>

<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_RumjacksAugust.jpg" />
  <figcaption >The Rumjacks Tour 2016 mit ausgewählten Daten vom August</figcaption>
</figure>


## Daten

Um die einzelnen Lokations auf der Karte meiner Anwendung zu zeigen, habe ich die Daten der Seite *songkick.com* beziehen können. Die API lieferte neben dem Datum auch gleich gut auswertbare Angaben zu den einzelnen Lokations und Events, die ich in das Projekt mit einfließen lassen konnte.


## Ausblick

Die vorrausgegangende Problemstellung der ich mich anfangs zu stellen versuchte war ja die Tourdaten von Bands auf einer Weltkarte zu visualisieren. Im Laufe des Semesters wurde klar, dass es nicht reicht allein den Kalender als Filteroption anzubieten. Es fehlt an einem regionalen Filter, mit dem ich meinen Standort angeben kann und einen Umkreis, in dem Daten angezeigt werden sollen. Der Standortfilter soll dabei aber auch genauso individuell wählbar sein wie die Zeitspanneneinstellung im Kalender. Somit soll gewährleistet werden, das zum Beispiel Studenten, die nicht in ihrer Heimat studieren, sich trotzdem dort stattfindende Konzerte anzeigen lassen kann um vielleicht seinen nächsten Besuch zu Hause zu planen.
Des weiteren wird es noch eine Anzeige von Informationen zu den Touren geben. Darin kann man Touren verschiedener Jahre vergleichen und sich auch Statistiken von einzelnen Monaten ausgeben lassen. Eine Heatmap soll dabei auch zeigen, ob verschiedene Bands regionale Vorlieben haben, sich etwa gern in einem speziellen Land oder einer speziellen Region aufhalten. Gerade bei national auftretenden Bands wird damit veranschaulicht, ob diese eher lokal auftreten oder ganze Touren durch das Land starten, oder sich Auftritte in einigen Städten rhytmisch wiederholen.

<figure>
  <img src="{{ site.urlimg }}/TourTracker/Tourtracker_Statistiken.jpg" />
  <figcaption >The Rumjacks Tour 2016 mit ausgewählten Daten vom August</figcaption>
</figure>
