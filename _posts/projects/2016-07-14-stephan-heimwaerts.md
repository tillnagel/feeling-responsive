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
    title: heimwaerts/heimwaerts_teaser.gif
    caption:
author: Stephan Hautzendorfer
---


Mitfahrgelegenheiten in Deutschland boomen:
Ungefähr alle vier Sekunden startet in Deutschland eine Mitfahrgelegenheit.  
Doch wo fahren Sie hin? Gibt es oft frequentierte Hauptstrecken oder Regionen die gar nicht von Mitfahrgelegenheiten befahren werden? Sind Mitfahrgelegenheiten wirklich so flexibel?
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

## Erste Datenvisualisierung
Für meinen ersten Datensatz wählte ich das DFB-Pokal-Wochenende bei dem Borussia Dortmund und
Bayern München in Berlin gegeneinander spielten. Meine Annahme war, dass
siginifikant mehr Mitfahrgelegenheiten für die Strecken Dortmund nach Berlin und München nach Berlin
in dem/den Tag/Tagen vor dem besagten Spiel angeboten würden.

<br/>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/dfb_monatsansicht.png" />
  <figcaption >Insgesamt werden mehr Mitfahrgelegenheiten mit Start in München angeboten. Eine Rhythmik der angebotenen Fahrten ist erkennbar.</figcaption>
</figure>

<br/>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/dfb_wochenenden.png" />
  <figcaption >Sichtbare Erhöhung der angebotenen Mitfahrgelegenheiten zum DFB-Pokal-Wochenende</figcaption>
</figure>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/dfb_feiertage.png" />
  <figcaption >An Tagen vor Feiertagen werden sehr viel mehr Fahrten angeboten.</figcaption>
</figure>
<br/>
Um ein aussagekräftiges Ergebnis zu erhalten, verglich ich das ausgewählte Wochenende mit
den anderen Wochenenden im Mai. Bei der Strecke zwischen München und Berlin stachen besonders
das Pfingstwochenende und der Mittwoch vor Christi Himmelfahrt heraus. Ein erstes Indiz, dass
Mitfahrgelegenheiten zum Heimfahren oder für kurze Wochenend-Trips genutzt werden könnten.
Später skalierte ich den Datensatz und bezog ihn auf die Stadt Halle (Saale).
Ich überprüfte die Strecken von Halle (Saale) in die einhundert größten deutschen Städte nach
Gesetzmäßigkeiten. Auch hier kam deutlich heraus, dass gerade am Freitag und Sonntag wesentlich
mehr Mitfahrgelegenheiten angeboten werden. Grundsätzlich kann festgehalten werden, dass die
Nähe der Stadt Einfluss auf die Anzahl der angebotenen Fahrten hat. So werden beispielsweise
sehr viele Fahrten nach Leipzig und Bitterfeld angeboten und wesentlich weniger nach Frankfurt/Main oder Stuttgart.     

<br/>
<figure>
<a href="{{ site.urlimg }}/heimwaerts/plakat_gross.jpg">
  <img src="{{ site.urlimg }}/heimwaerts/plakat_klein.png" /></a>
  <figcaption >Angebotene Mitfahrgelegenheiten von www.blablacar.de zwischen Halle (Saale) und Deutschlands einhundert größten Städten, sowie ausgewählten Städten im Einzugsgebiet vom 01.05.2016 — 31.05.2016. Geordnet nach Anzahl der Einwohner.</figcaption>
</figure>
<br/>
Nach dem Herausstellen erster Zusammenhänge, habe ich einen ausgewählten Datensatz auf eine geografische Karte übertragen.
Ich wählte dreißig Städte über ganz Deutschland verteilt und prüfte deren Hin- und Rückverbindung nach Halle (Saale) auf
(Un-)Regelmäßigkeiten. Ich konnte herausfinden, dass es vielbefahrene Hauptstrecken gibt. Über diese Form der Visualisierung
lässt sich zudem ein Zusammenhang zwischen der Entfernung zum Zielort und der Anzahl der Fahrten feststellen. Liegt Halle (Saale)
zwischen einem Startort und Berlin, so ist die Strecke wesentlich häufiger befahren. Beispielsweise liegen Stuttgart und
München sehr weit von Halle (Saale) entfernt, weisen jedoch eine hohe Anzahl an Fahrten auf, was sich über die
Autobahnroute nach Berlin erklären lässt.
<br/>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/flowchart_deutschland.png" />
  <figcaption >Verbindungen in der ersten Mai-Woche 2016 von Halle (Saale) zu 30 ausgewählten Städten in Deutschland</figcaption>
</figure>
<br/>
## Vizualisierungsprozess
Es sollte eine Browser-Anwendung entstehen in der die Nutzer die Möglichkeit haben
verschiedene Tage miteinander zu vergleichen. Der Nutzer sollte die Möglichkeit bekommen
von allgemeinen Daten, wie der Anzahl der gesamten Fahrten von einem Tag, zu detaillierteren
Daten zu gelangen, wie eine Aufschlüsselung zu welcher Tageszeit auf eine bestimmte Strecke
befahren wird.     
<br/>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/visualisierung.jpg" />
  <figcaption >Visualisierungsprinzip</figcaption>
</figure>
<br/>

Um dies darzustellen sieht der Nutzer zum Start der Applikation eine Deutschlandkarte mit den
Fahrten des aktuellen Tages. Die Karte ist zoombar und kann mit der Maus bewegt werden. Fährt man nun über Städte oder
einzelne Verbindungen, werden diese hervorgehoben. Wählt man diese aus, so soll man spezielle Daten für
die getroffene Auswahl bekommen. Um die Auswahl mit weiteren Tagen zu vergleichen, klickt man auf das Hinzufügen einer
Karte. Es soll möglich sein mehrere Karten gleichzeitig miteinander zu vergleichen. Nun ist es auch möglich in jeder Karte
das gewünschte Datum einzustellen.     


## Prototyp
Der Prototyp wurde in D3.js umgesetzt und kann mit dem Browser geöffnet werden. Zur Entwicklung wurde Google Chrome Version 51+ genutzt.
Er stellt die Entwicklung des Projekts von April – Juli 2016 dar.
<br/>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/prototyp_start.gif" />
  <figcaption >Startbildschirm des Prototyps. Aufbau der Grafik an verschiedenen Tagen.</figcaption>
</figure>
<br/>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/prototyp_zoom.gif" />
  <figcaption >Die Zoom-Funktion ermöglicht eine bessere Selektierung einzelner Strecken und Städte</figcaption>
</figure>
<br/>
<figure>
  <img src="{{ site.urlimg }}/heimwaerts/prototyp_vergleich.gif" />
  <figcaption >Das Hinzufügen von Karten und die Auswahl verschiedener Tage</figcaption>
</figure>
