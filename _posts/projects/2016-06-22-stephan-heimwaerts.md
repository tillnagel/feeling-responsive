---
layout: page
title:  "heimwaerts"
subheadline: Atlas der Mitfahrgelegenheiten
teaser: " <em>heimwaerts</em> ist kein Ort,
heimwaerts ist eine Richtung.
Es ist ein Gefühl, eine Mission, ein Glaube.
heimwaerts kann es nicht nur einmal geben,
doch kennt nicht jeder sein heimwaerts.
heimwaerts fahren wir am liebsten.
heimwaerts erzählt Geschichten.
Das ist unser tägliches heimwaerts."
header: no
show_meta: false
categories:
    - projects
image:
    title: heimwaerts_teaser.gif
    caption: heimwaerts logo mit animierten verbindungen
author: Stephan Hautzendorfer
---


Mitfahrgelegenheiten in Deutschland boomen:
Ungefähr alle vier Sekunden startet in Deutschland eine Mitfahrgelegenheit.  
Doch wo fahren Sie hin? Gibt es oft frequentierte Hauptstrecken oder Regionen die gar nicht von Mitfahrgelegenheiten befahren werden? Sind die Mitfahrgelegenheiten wirklich so flexibel?
heimwaerts antwortet auf diese Fragen als Atlas der Mitfahrgelegenheiten. Mithilfe der Browser-
Applikation können Tage miteinander verglichen werden ­— deutschlandweit oder einzelne Städte.


## Ausgangslage
Mitfahrgelegenheiten sehen sich als ein Gegenentwurf zu den statischen Fahrplänen von Bahn und Fernbus.
Vier große Portale aus meine Analyse vermitteln uns neben einer preiswerten Fahrt, Flexibilität und
dauerhaften Anschluss in alle Ecken der Bundesrepublik. Was für Verbindungen zwischen Großstädten gilt,
geht bei näherer Betrachtung aber nicht mehr ganz auf.
Ist es dennoch möglich eine fahrplanähnliche Prognose für Mitfahrgelegenheiten aufzustellen oder
unterliegt der Kosmos für Mitfahrgelegenheiten wirklich keinen Gesetzen?
Mit meiner Visualisierung möchte ich die Andeutungen der Mitfahr-Portale überprüfen und ggf. revidieren.

## Daten
Eine offene Datenbank oder verfügbare API liefert leider kein Portal. Meine verwendeten Daten mussten
direkt von den Webseiten bezogen werden. Für eine aussagekräftige Visualisierung reichte es für das heimwaerts-Projekt
die Abfahrtort und -zeit, Ankunftsort und angebotene Fahrten am gesamten Tag zu verwenden.
Die Genauigkeit der Daten kann leider nicht überprüft werden. Ob eine Fahrt wirklich stattfand
oder ob der Ankunftsort auch das letzte Ziel der Fahrt war, muss leider unbeantwortet bleiben.

## Daten visualisieren
Für meinen ersten Datensatz wählte ich das DFB-Pokal-Wochenende bei dem Borussia Dortmund und
Bayern München in Berlin gegeneinander spielten. Meine Annahme war, dass
siginifikant mehr Mitfahrgelegenheiten für die Strecken Dortmund nach Berlin und München nach Berlin
in dem/den Tag/Tagen vor dem besagten Spiel angeboten würden.

<figure>
  <img src="{{ site.urlimg }}/heimwaerts/dfb_monatsansicht.png" />
  <figcaption >Insgesamt werden mehr Mitfahrgelegenheiten mit Start in München angeboten. Zusätzlich ist bereits eine Rhythmik in den angebotenen Fahrten erkennbar.</figcaption>
</figure>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/dfb_wochenenden.png" />
  <figcaption >sichtbare Erhöhung der Anzahl der angebotenen Mitfahrgelegenheiten zum DFB-Pokal-Wochenende</figcaption>
</figure>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/dfb_feiertage.png" />
  <figcaption >An den Tagen vor Feiertagen werden sehr viel mehr Fahrten angeboten.</figcaption>
</figure>

Um ein aussagekräftiges Ergebnis zu erhalten, verglich ich das ausgewählte Wochenende mit
den anderen Wochenenden im Mai. Bei der Strecke zwischen München und Berlin stachen besonders
das Pfingstwochenende und der Mittwoch vor Christi Himmelfahrt heraus. Ein erstes Indiz, dass
Mitfahrgelegenheiten zum Heimfahren oder für kurze Wochenend-Trips genutzt werden könnten.





## Visualization Design
*cf. city flows* has three viewing modes, all visualizing trips of rented bikes, but focusing on different levels of spatial and temporal granularity of cycling mobility:

* The citywide view aggregates all trajectories of bike-sharing trips for a given day and animates the trails for trips at a given time.
* In the station view only the bike trips to and from a selected station are shown, allowing the distinction between incoming and outgoing.
* A small-multiple view visualizes spatiotemporal patterns for three selected stations each in an exploded view that separates incoming from outgoing and morning from afternoon/evening trips.

<figure>
<a href="{{ site.urlimg }}/cf-view2-london-draft.jpg">
  <img src="{{ site.urlimg }}/cf-view2-london-draft.jpg" />
  <figcaption >Angebotene Mitfahrgelegenheiten von www.blablacar.de zwischen Halle (Saale) und Deutschlands einhundert größten Städten, sowie ausgewählten Städten im Einzugsgebiet Halle (Saale) vom 01.05.2016 — 31.05.2016.
Geordnet nach Anzahl der Einwohner.</figcaption>
</figure>


## Design Prozess
In our process of exploring the bike data, and designing the visualizations we created lots of visual experiments. Some of those we share below.


## Daten
