---
layout: page
title:  "Farbe Text Emotion"
subheadline: Spiegeln Bilder Emotionen in Texten wider?
teaser: "<em>Farbe Text Emotion</em> analysiert Artikel und Bilder der New York Times, und visualisert emotionale Werte der Texte in Verbindung mit Bildanalysen."
header: no
show_meta: false
categories:
    - projects
image:
    title: marcel2.jpg
    caption: Glyphen zeigen die Farbpaletten von Bildern in verschiedenen Artikeln.
author: Marcel Wiessler
---

Die Arbeit untersucht, ob Bilder die sie umgebenden Texte widerspiegeln.
Haben Bilder auf Instagram gesättigtere Farben, wenn sie mit eher fröhlichen Tags ausgezeichnet werden? Teilen Instagram Nutzer eher schwarz weiß Bilder, wenn sie traurig sind? Gibt es einen Unterschied zwischen der öffentlichen Emotionalität sozialer Medien und der professioneller Nachrichtenportalen, die zur Tonalität des Artikels passt?

Die Arbeit untersucht verschiedene hypothetische Zusammenhäng zwischen Bild- und Textinformationen. Nach der Recherche technischer Möglichkeiten beschränkt sich die Arbeit auf eine Farbauswertung der Bilder. Algorithmisch extrahierte Farbpaletten werden als meßbare Stellvertreter verwendet, um gewisse Aussagen über die Emotionalität der Bilder treffen zu können.
Die Stimmung der Texte wird mit Hilfe sogenannter Sentiment Analysis Software errechnet, die Wörter und Sätze Werte bestimmter emotionale Kategorien zuordnet.

Aufgrund der offenen Fragestellung und der komplexen Materie geht diese Arbeit ergebnisoffen und experimentell vor. Die Visualisierungen sind nicht nur Mittel zur Kommunikation der Ergebnisse sondern maßgeblicher Bestandteil der Analyse und der Auseinandersetzung mit dem Medium.

## Daten und Analyse

#### New York Times
Die New York Times wurde als eine der ältesten und größten Tageszeitungen in Amerika ausgewählt, da sie neben ihrer hohen Gesamtauflage (wochentags 1.124.700 Druckexemplare) auch eine der meistbesuchten Nachrichtenseiten weltweit ist (Platz 5 mit 41.6 Mio monatlichen Besuchern) . Darüber hinaus bietet die New York Times eine sehr gute API an, die u.a. Zugriff auf alle veröffentlichten Artikel zwischen 1851 und heute ermöglicht. Bei der Arbeit mit Bildmaterial muss allerdings erwähnt werden, dass ab ca. 2012 die Artikelbilder online nicht mehr verfügbar sind.

Alle Daten wurden mithilfe einer in Unity/C# entwickelten Anwendung heruntergeladen.

#### Natural Language Processing
Verwendet für die Text-Analyse der finalen Ergebnisse wurde der Tone Analyzer Service von IBM Watson. 
Der Tone Analyzer nutzt Sprachanalyse, um drei Formen von Umgangston in Texten zu erkennen: emotion, social tone und language tone. Für emotion vergibt er Werte in den Kategorien anger, joy, fear, sadness 
und disgust . social tone besteht aus den Kategorien openess (Offenheit), conscientiousness (Pflichtgefühl), extroversion (Extroversion), agreeableness (Verträglichkeit) und emotional range (emotionale Bandbreite). language tone umfasst Werte für confident (überzeugt), analytical (analytisch) sowie tentative (zögernd). Die vergebenen Werte liegen jeweils im Bereich von 0 - 1. Alle Werte werden sowohl für den gesamten Text als auch satzweise vergeben. 

#### Extrahierung von Farbpaletten
Ein in Processing entwickeltes Programm teilt das Farbspektrum eines Bildes zunächst in 6 gleich große Farbtonbereiche. Jeder Farbton wird anschließend in 4 weitere Helligkeitsstufen unterteilt. Um minimale Pixel- bzw. Objektivfehler zu vermeiden, werden mehrere einzelne Pixel in einem Cluster zusammengefasst und der errechnete Durchschnittsfarbwert einem Bereich zugeordnet. Nachdem alle Cluster einem Bereich zugeordnet wurden, werden die Bereiche ihrer  Größe nach geordnet, um eine relative Verteilung der Farben (die Farbpalette) eines Bildes zu erhalten.

## Prozess

Ein Prozess Video fasst die Versuche und Experimente, die im Laufe des Projektes entstanden sind, zusammen. Insgesamt sind in dem Projekt ca. 1385 Processing Renderings entstanden. Erste Versuche visualisieren Bilder und Texte von Instagram. Im Verlauf des Projektes wurde die Datenquelle jedoch auf Nachrichtenartikeln der New York Times (zunächst 2013, dann 2015) geändert. Im Video wird die Datenquelle durch das jeweilige Logo rechts unten im Bild angezeigt.

Alle Grafiken wurden in Processing erzeugt:

<div class="flex-video">
<iframe src="https://player.vimeo.com/video/173058434" width="640" height="360" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
</div>

Die Abbildungen unten verdeutlichen die Darstellung der Farbpaletten in chronologischer Folge anhand weniger Artikel aus dem Jahr 2013. Die Farbkreise werden hier anhand der Farbmenge je Bild skaliert:

<figure>
<a href="{{ site.urlimg }}/farbetextemotion/beispiele_2013.jpg">
  <img src="{{ site.urlimg }}/farbetextemotion/beispiele_2013-preview.jpg" /></a>
</figure>

<figure>
<a href="{{ site.urlimg }}/farbetextemotion/beispiele_2013-2.jpg">
  <img src="{{ site.urlimg }}/farbetextemotion/beispiele_2013-2-preview.jpg" /></a>
</figure>

## Ergebnisse

Entstanden sind zwei großformatige Plakate, deren Abbildungen und Grafiken auf vorherigen Experimenten mit dem Datensatz der New York Times basieren. Während die Experimente und erste Versionen der Plakate auf Daten von 2013 basieren, nutzen die Endergebnisse aufgrund der höheren Aktualität Daten von 2015. 

Das erste Plakat dient der Einführung in die Thematik und den Hintergrund der Arbeit. Es gibt außerdem einen Überblick über die verschiedenen Ansätze und Rohdaten. Dabei werden Farbpaletten, Themen und Emotionen in chronologischer Reihenfolge präsentiert. 

<figure>
<a href="{{ site.urlimg }}/farbetextemotion/plakat1-big.jpg">
  <img src="{{ site.urlimg }}/farbetextemotion/plakat1-preview.jpg" /></a>
  <figcaption>Projektergebnis Plakat 1, 200x92cm</figcaption>
</figure>

Das zweite Plakat zeigt nach Kategorien geordnete Worthäufung und ermöglicht einen tieferen Einblick und Vergleiche von Themen innerhalb verschiedener Kategorien.

<figure>
<a href="http://gaisterhand.de/wp-content/uploads/2016/07/Plakat-3.6-300x92-big.jpg">
  <img src="{{ site.urlimg }}/farbetextemotion/plakat2-preview.jpg" /></a>
  <figcaption>Projektergebnis Plakat 2, 300x92cm</figcaption>
</figure>

Das zweite Plakat beschränkt sich auf eine Darstellung der Worthäufungen, da diese Visualisierung den größten Einblick in für die New York Times scheinbar wichtige Themen ermöglicht und gleichzeitig sie in Verbindung mit Farben und Emotionen kompakt zusammenfasst. 

Anstelle der zeitlichen Ordnung wie auf dem ersten Plakat werden die Worthäufungen nun jedoch nach Kategorien aufgeteilt dargestellt. Beispielsweise ist in der Kategorie „europe“ das häufigst gebrauchte Substantiv „migrants“.

<figure>
  <img src="{{ site.urlimg }}/farbetextemotion/plakat2-howtoread.jpg" />
</figure>

<figure>
<a href="{{ site.urlimg }}/farbetextemotion/europe.jpg">
  <img src="{{ site.urlimg }}/farbetextemotion/europe-preview.jpg" /></a>
  <figcaption>Meist genutzte Wörter (Adjektive, Substantive, Verben) in der Kategorie "europe" in den Artikeln der New York Times 2015</figcaption>
</figure>

Gleichzeitig wird die Visualisierung ergänzt durch häufig vorhergehende sowie nachfolgende Adjektive, Nomen oder Verben. Dies hat den Vorteil, dass in verschiedenen Kategorien auftretende Worte, beispielsweise das Wort „leader“, im Kontext betrachtet und verglichen werden kann.

<a href="http://www.marcelwiessler.de" target="_blank">www.marcelwiessler.de</a>


<a href="https://twitter.com/share" class="twitter-share-button">Tweet</a>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+'://platform.twitter.com/widgets.js';fjs.p	arentNode.insertBefore(js,fjs);}}(document, 'script', 'twitter-wjs');</script>



