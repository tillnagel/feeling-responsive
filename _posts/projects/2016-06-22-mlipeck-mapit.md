---
layout: page
title:  "Map it"
subheadline: Hierarchische Visualisierung besuchter Orte.
teaser: "Eine neuartige Visualisierung von besuchten Orten als hierarchische Circular Tree Map, um eine persönliche Karte zu erstellen."
header: no
show_meta: false
categories:
    - projects
image:
    title: mapit.jpg
    caption: Erste Entwurf von Map it
author: Matthias Lipeck
---

Zur Zeit gibt es einige eindrucksvolle Projekte, im Bereich personenbezogener Geodaten, wie [visits](http://v.isits.in) oder [Shifted Maps](http://shifted-maps.com). Beide Projekte inspirierten durch ihre jeweiligen besonderen Art der Datenaufbereitung und der damit verbundenen Zugänglichkeit für den Betrachter.


„Map it“ stellt die von dem Nutzer besuchten Orte dar. Dabei wird eine Darstellungsart genutzt, die auf Wegebeziehungen zwischen den Orten verzichtet und dadurch das Hauptaugenmerk auf die besuchten Orte legt.
Dadurch entsteht eine neue Karte für den Nutzer - seine Karte. Diese Form der Darstellung ist inspiriert durch Guy Debord, dem es nicht um die exakte Abbildung der Entfernungen zwischen Orten und ihren räumlichen Positionen zueinander ging, sondern um die erreichten Orte, die in einer Gesamtkarte dargestellt werden. Mit dieser Idee der Kartendarstellung ist Debord eine wichtige Person der Psychogeographie.

„Map it“ nutzt Daten, welche durch die App „Moves“ auf dem Smartphone erfasst werden. Die besuchten Orte werden anschließend in der Circular TreeMap visualisiert. Dabei werden die Orte in einer hierarchische Darstellung geclustert. Somit beinhaltet der äußerste Kreis alle besuchten Orte, während die Größe jedes einzelnen Kreises den Gesamtaufenthalt des jeweiligen Ortes visualisiert. Ein Beispiel der hierarchischen Darstellung: Land → Region → Stadt → Stadtteile → einzelne Orte. Die Größe der Kreise in der Circular TreeMap ist proportional abhängig von der Häufigkeit oder der Dauer der jeweiligen besuchten Orte. Das heißt, je öfter oder je länger ein Ort besucht wird, um so größer ist der Kreis und die ihm zu Grunde liegenden geographischen Karten.

Die in der App Moves gesammelten Daten werden über eine API ausgelesen und auf einer Webseite in der Circular TreeMap aufgearbeitet und ausgegeben. Die Webseite bietet neben der graphischen Darstellung auch die Möglichkeit der Interaktion, wie zum Beispiel das Zoomen auf die jeweiligen besuchten Orte oder das Abrufen von weiteren Informationen wie die Dauer sowie die Anzahl der Besuche oder die Zeiträume der Datenaufzeichnung auf die sich die Werte beziehen.

„Map it“ wurde prototypisch mit Processing, Unfolding Maps und D3.js umgesetzt.

<!--
<figure>
  <img src="{{ site.urlimg }}/radialtreeplaces.jpg" />
  <figcaption >Eine Bildbeschreibung</figcaption>
</figure>
-->
