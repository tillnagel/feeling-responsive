---
layout: page
title:  "SurroundFound"
subheadline: Lebe deinen Moment.
teaser: "Lebe deinen Moment."
header: no
show_meta: false
categories:
    - projects
image:
    title: SurroundFound/Mockup-01.png
    caption: Mockup
author: Melanie Miksch &amp; Sophie Parschat
---

Du möchtest etwas unternehmen, doch weißt nicht wo und was? Bei „SurroundFound“ geht es um das Hier und Jetzt, um den Moment. Stoppe nicht deine Unternehmungslust mit dem Durchsuchen langer Listen. Lerne Deine Stadt oder noch nicht gesehene Orte kennen. Finde und entdecke deinen Weg zu Veranstaltungen in Deiner Nähe. Du hast die Möglichkeit zwischen verschiedenen Kategorien zu schalten und Dein Ziel individuell zu bestimmen. Zusätzlich geben Dir Isolines die grobe Entfernung an. Somit kannst du Entscheiden welche Distanz Du auf Dich nehmen möchtest. Ist die Entscheidung gefallen wirst Du über eine linearisierte Wegdarstellung geleitet.Kreuzungen an denen Abgebogen werden muss, sind durch Kreise gekennzeichent, welche die Farbigkeit der Isolines aufgreifen. Sobald eine Aktion statt gefunden hat, richtet sich die Route neu nach dem Nutzer aus. Entlang eines Weges befinden sich oftmals wichtige Gebäude, Sehenswürdigkeiten oder interessante Orte. Diese orientieren sich zum einen an Deiner Sichtachse und zum anderen an der Entfernung zur Route und dienen zur visuellen Orientierung beziehungsweise zum
Kennenlernen der Stadt.
<br />
<figure>
  <img src="{{ site.urlimg }}/SurroundFound/LogoSchrift-01-01.png" />
  <figcaption >Schriftlogo</figcaption>
</figure>


## Zielfragen
<br />
* Wo ist meine nächste Veranstaltung?<br />
* Wie weit will ich weg sein von meinem Standpunkt?<br />
* Was will ich überhaupt?<br />
* Gibt es noch Alternativen?<br />
* Wo sind meine Freunde?<br />
<br />


## Experimentierphase
<br />
Von Anfang an war uns klar, dass wir weg wollten von Listen und eine visuelle Orientierung über ein Kartensystem schaffen wollten.<br />
Zu Anfang hatten wir die Idee eine 3D-Karte zu gestalten. Eine daraus resultierende Idee war eine Kombination aus 2D und 3D. Eine vereinfachte Karte in der unsere Landmarks als 3D Objekte gezeigt werden. Diese Idee tauchte wärend der Design- und Konzeptphase immer mal wieder auf, wurde jedoch verworfen.
<br />
<figure>
  <img src="{{ site.urlimg }}/SurroundFound/SurroundFoundExperiement01.png" />
  <figcaption >Experimente zur 3D-Karte</figcaption>
</figure>


<br />
Wir haben für uns festgestellt dass es in Anbetracht der Zeit und der wenigen Daten von Halle, uns nicht möglich gewesen wäre Modelle zu gestalten die unseren Vorstellungen entsprochen hätten. Wir sind noch einmal zurück gegangen und haben überlegt welche anderen Gestaltungsprinzipien wir noch in Betracht ziehen könnten.
<br />
<figure>
  <img src="{{ site.urlimg }}/SurroundFound/SurroundFoundExperiement012.png" />
  <figcaption >weitere Ideen mit anderen Gestaltungsprinzipien</figcaption>
</figure>


<br />
Weiterhin wurden in der Experimentierphase Fragen angesprochen wie das Filtersystem, Marker, Farbkonzepte und ähnliches und nach Lösungsansätzen gesucht.
<br />
<figure>
  <img src="{{ site.urlimg }}/SurroundFound/Experimente_03.png" />
  <figcaption >Erste Entwürfe für den Kartenstil </figcaption>
</figure>


## Daten
<br />
Die Daten stammen von Overpass Turbo, welches uns erlaubten Information über verschiedene Lokalitäten
aus verschiedenen Kategorien zu beziehen. Weginformationen und Isolineinformationen stammen von einer Here Maps API.
<BR />
<figure>
  <img src="{{ site.urlimg }}/SurroundFound/Daten-01.png" />
  <figcaption >Beispiele der Daten</figcaption>
</figure>


## Design
<br />
Unser Layout teilt sich in zwei Bereiche. Auf der linken Seite eine realistische Karte mit Filtersystem, auf der rechten eine linearisierte Route. Auf beiden Karten werden die Entfernungen zwischen Standpunkt und Ziel sowie verschiedene Marker gezeigt.
<br />

<figure>
  <img src="{{ site.urlimg }}/SurroundFound/Kartenstil02.png" />
  <figcaption >Entwurf Kartenstil</figcaption>
</figure>

<figure>
  <img src="{{ site.urlimg }}/SurroundFound/Kartenstil.png" />
  <figcaption >Entwurf Kartenstil</figcaption>
</figure>

## Filtersystem
<br />
Das Filtersystem ermöglicht es sich sein eigenes Ziel festzulegen. Auf der linken Seite befindet sich die Button Bar, welche die verschiedenen Kategorien bereitstellt. Sobald eine der Kategorien ausgewählt wurde, werden die Marker eingeblendet. Diese geben einen Überblick der bevorstehenden Veranstaltungen. Nun können über Hover die Informationen angezeigt werden. Ist das passende Event gefunden, können sie sich nun den Weg dorthin generieren lassen.


* Roter Marker markiert deinen Standpunkt
* Orangene Marker zeigen Veranstaltungen in deiner Nähe
* Isolines geben die Entfernung vom Standpunkt zum <br />
  Ziel in 5 Minuten Abschnitten an
<br />
<figure>
  <img src="{{ site.urlimg }}/SurroundFound/Filtersystem02.png" />
  <figcaption >Filtersystem</figcaption>
</figure>


## Linearer Weg
<br />
Der Lineare Weg ist die zweite Darstellung unserer Anwendung. Sie orientiert sich an diejenigen Kreuzungen an denen abgebogen werden muss. Diese werden durch farbige Punkte dargestellt, welche sich in ihrer Farbigkeit nach den Isolines richten. Andernfalls werden sie als einfache Linien auf dem Weg markiert. Sobald ein Maneuver erreicht ist, richtet sich die Karte neu nach dem Nutzer aus.


* Kreise auf der Strecke sind Hinweise, wann abgebogen werden muss
* Farbigkeit der Kreise gibt die Entfernung zum Ziel an
* Linien auf der Strecke markieren nicht benutzte Kreuzungen
* Grüne Marker zeigen wichtige Landmarks auf

<figure>
  <img src="{{ site.urlimg }}/SurroundFound/Linear.png" />
  <figcaption >Linearer Weg</figcaption>
</figure>


## Landmarks
<br />
Die Landmarks dienen zum einen zur visuellen Orientierung und zum anderen zum
neuentdecken beziehungsweise kennenlernen der Stadt. Somit können sie auch als
optionaler Umweg fungieren.


* zeigen wichtige Gebäude, Parks oder Sehenwürdigkeiten <br />
  entlang deiner Sichtachse

  <figure>
    <img src="{{ site.urlimg }}/SurroundFound/Landmark_Tap.png" />
    <figcaption >Landsmarks</figcaption>
  </figure>
