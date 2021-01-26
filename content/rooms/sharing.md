---
title: "Räume teilen"
date: 2020-07-02T21:23:14+02:00
chapter: true
draft: false
weight: 40
---
# Räume teilen und publik machen

Jeder Raum hat eine Adresse, die man in den Raumeinstellungen unter dem Reiter Erweitert finden kann, bspw.

!aen6iekahv8Pi0zohf:tu-dresden.de

Da diese kryptische Adresse aber von Menschen nicht leicht gelesen werden kann, können Raumadressen vergeben werden, die von Menschen gelesen werden können. Dies ist nur in Räumen nötig, die man an anderen Stellen publik machen möchte.

Entweder durch global veröffentlichte Adressen (auffindbar von Benutzenden in anderen Servern - sinnvoll bei Themen, die über die TU Dresden hinausgehen) oder durch eine lokale Adresse, die nur innerhalb des Matrix-Heimatservers an der TU Dresden gilt.

Für den häufigeren Fall der gewünschten lokalen Adresse in die Raumeinstellungen unter dem Reiter Allgemein auf „Show more“ unter Local Addresses klicken:

![Raumeinstellungen mit dem mehr anzeigen ausgewählt](/images/01_Sharing_de.png)

Anschließend  kann in der „Room alias“ Zeile ein wiedererkennbarer Name dieser Raumverknüpfung vergeben werden (keine Leerzeichen!):

![Raumeinstellungen mit dem lokale Adressen ausgewählt](/images/02_Sharing_de.png)

Es können auch verschiedene Adressen vergeben werden. Sollte die Raumadresse im Raum-Verzeichnis des Matrix-Heimatservers der TU Dresden veröffentlicht werden sollen, kann dies durch den folgend gezeigten Schalter und die Auswahl der Primären Adresse im Drop-Down-Menü erfolgen:

![Raumeinstellungen mit dem öffentliche Raumadresse ausgewählt](/images/03_Sharing_de.png)

Die Raumadresse hat dann folgende Struktur

#Raumadressname:tu-dresden.de

Wenn innerhalb von Matrix auf einen anderen Raum verlinkt werden soll, kann dies einfach durch (beginnendes) Eintippen in das Nachrichtenfeld von
```
#Raumadressname:tu-dresden.de
```
geschehen. Ist man selber Mitglied in dem Raum, so erscheinen automatisch Vorschläge. Dies ist dann ein spezieller Hyperlink innerhalb von Matrix, der auch direkt im Client der empfangenden Person (mit einem Mausklick) genutzt werden kann.


Weiterhin resultiert aus der vergebenen Raumadresse eine Internetadresse (URL)

https://matrix.tu-dresden.de/#/room/#Raumadressname:tu-dresden.de

Diese kann leicht in der Öffentlichkeit bzw. an die Zielgruppe verteilt werden, öffnet sich allerdings in Element Web, nich in einem ggf. installiertem Element Desktop.

![Teilensymbol in der Chatansicht des Raums makiert](/images/04_Sharing-Button_de.png)

{{% notice note %}}
Das Teilen-Symbol oben rechts in jedem Raum, bietet auch einen matrix.to-Link an, sowie einen QR-Code und verschiedene soziale Netzwerke. Der matrix.to- Link führt auf eine Seite, auf der ausgewählt werden kann, wie der Link geöffnet werden soll. So kann z.B. der installierte Element-Client verwendet werden, oder ausgewählt werden, über welchen Heimserver der Raum betreten werden soll. 
{{% /notice %}}


