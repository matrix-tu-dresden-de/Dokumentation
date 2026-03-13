---
title: "Räume teilen"
date: 2020-07-02T21:23:14+02:00
chapter: true
draft: false
weight: 40
---
# Räume teilen und publik machen

Jeder Raum hat eine Adresse, die man in den Raumeinstellungen unter dem Reiter Erweitert finden kann, bspw.

<p style="text-align: center; font-style: italic;">!aen6iekahv8Pi0zohf:tu-dresden.de</p>

Da diese kryptische Adresse aber von Menschen nicht leicht gelesen werden kann, können Raumadressen vergeben werden, die von Menschen besser gelesen werden können. Dies ist nur in Räumen nötig, die man an anderen Stellen publik machen möchte.

Entweder durch global veröffentlichte Adressen (auffindbar von Benutzenden in anderen Servern - sinnvoll bei Themen, die über die TU Dresden hinausgehen) oder durch eine lokale Adresse, die nur innerhalb des Matrix Homeservers an der TU Dresden gilt.

{{% notice note %}}
Um eine globale Adresse zu veröffentlichen, muss diese zu aller erst als lokale Adresse erstellt worden sein. **Das heißt in beiden Fällen ist es notwendig eine lokale Adresse zu erstellen.**
{{% /notice %}}

Um eine lokale Adresse einzurichten ist in die Raumeinstellungen unter dem Reiter Allgemein auf „Mehr Anzeigen“ unter Lokale Adressen zu klicken:

![Raumeinstellungen mit dem mehr anzeigen ausgewählt](/images/01_Sharing_de.png)

Anschließend kann in der Zeile "Raumadresse" ein wiedererkennbarer Name vergeben werden (keine Leerzeichen!):

![Raumeinstellungen mit dem lokale Adressen ausgewählt](/images/02_Sharing_de.png)

Es können auch verschiedene Adressen vergeben werden. Sollte die Raumadresse im Raum-Verzeichnis des Matrix Homeservers der TU Dresden veröffentlicht werden sollen, kann dies durch den folgend gezeigten Schalter und die Auswahl der Primären Adresse im Drop-Down-Menü erfolgen:

![Raumeinstellungen mit dem öffentliche Raumadresse ausgewählt](/images/03_Sharing_de.png)

Die Raumadresse hat dann folgende Struktur

<p style="text-align: center; font-style: italic;">#&lt;raumadressname&gt;:tu-dresden.de</p>

Wenn innerhalb von Matrix auf einen anderen Raum verlinkt werden soll, kann dies einfach durch (beginnendes) Eintippen in das Nachrichtenfeld von `#<raumadressname>:tu-dresden.de` geschehen. Ist man selbst Mitglied in dem Raum, so erscheinen automatisch Vorschläge. Dies ist dann ein spezieller Hyperlink innerhalb von Matrix, der auch direkt im Client der empfangenden Person (mit einem Mausklick) genutzt werden kann.

Erhält man solche Adressen auf anderem Wege (z.B. via E-Mail) hilft es, diese in einen persönlichen Notizraum (selbst angelegter Raum ohne weitere Personen) zu senden. Anschließend kann man dann bequem auf diesen sich ergebenden Raumlink klicken.

Das Teilen-Symbol oben rechts in jedem Raum, bietet einen matrix.to-Link an, sowie einen QR-Code und verschiedene soziale Netzwerke. Der matrix.to- Link führt auf eine Seite, auf der ausgewählt werden kann, wie der Link geöffnet werden soll. So kann z.B. der installierte Client Element Desktop verwendet werden, oder ausgewählt werden, über welchen Heimserver der Raum betreten werden soll.

![Teilensymbol in der Chatansicht des Raums makiert](/images/04_Sharing-Button_de.png)

<!--
```
https://matrix.to/#/#Raumadressname:tu-dresden.de?via=tu-dresden.de
```
-->

Weiterhin kann man aus der vergebenen Raumadresse eine Internetadresse (URL) nach folgender Struktur konstruieren:

<p style="text-align: center; font-style: italic;">https://matrix.tu-dresden.de/#/room/#&lt;raumadressname&gt;:tu-dresden.de</p>

Diese kann auch leicht in der Öffentlichkeit bzw. an die Zielgruppe verteilt werden, **öffnet sich allerdings nur in Element Web**, nicht in einem ggf. installiertem Element Desktop. Universeller (insbesondere für die große Gruppe an Personen mit Element Desktop) und inzwischen empfehlenswerter ist daher der zuvor beschriebene Weg mit dem matrix.to-Link.
