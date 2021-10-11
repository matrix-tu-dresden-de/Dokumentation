---
menutitle: "Blog/News"
title: "Blog"
date: 2020-01-02T21:26:25+02:00
draft: false
weight: 200
---


***
#### Spaces{#spaces}

Mit den aktuellsten Element-Clients kann man Beta-Tests der Spaces durchführen. Diese sind im Client (Beta!) zu aktivieren. 






#### TU Dresden hat mehr als 20.000 Matrix User (#20000)








Pull Request MDAD worker

Erfolgreicher Beitrag an der Matrix-Entwicklung durch die TU Dresden

Am Wochenende wurde ein Pull Request (Vorschlag für verbesserten Programmcode) mit der Nummer 456 innerhalb des Matrix-Docker-Ansible-Deploy Paketes (MDAD) angenommen und in den Master-Zweig übernommen, der von der TU Dresden angestoßen und maßgeblich in den letzten 10 Monaten mitentwickelt wurde.

Die Code-Anpassungen, die den Dresdner Matrix-Dienst für mittlerweile > 18.000 User stabil durch gezielte Lastverteilung auf sogenannte synapse-worker ermöglichen, wurden durch .... Personen kollaborativ weiterentwickelt und stehen nun allen MDAD-Nutzenden weltweit frei zur Verfügung.

Die TU Dresden hat hier einmal mehr bewiesen, dass die Förderung von freier Software nicht nur durch die finanzielle Unterstützung einer Gruppe von Entwickelnden (Beispiel ?) oder der direkten Beauftragung für die Entwicklung neuer Funktionen (Beispiel LibreOffice (Link) oder Okular (Link)) möglich ist. Wenn kaum Geld vorhanden ist, dann ist das Zurückspeisen von eigenen Weiterentwicklungen an die globale Community das Mindeste. 

Die Ausnutzung von synapse-worker durch Pull Request 456 versetzt andere große Institutionen (z.B. die vielen Hochschulen, die auch Matrix einsetzen) in die Lage eine stabile, skalierbare Instanz zu betreiben.





Hochschulen-Artikel (Element), Uni Linz



#### 29.03.2021 Relogin

Durch eine Aktualisierung am Matrix Server haben sich die Orte für Mediendateien verändert. Clients, die seit einem Zeitpunkt vor dem 28.03.2021 angemeldet sind, können dieses Problem nur durch ein Ab- und erneutes Anmelden lösen. Damit dabei keine früheren verschlüsselten Nachrichten verloren gehen ist dringend auf die [in den FAQ beschriebene Prozedur]({{< relref "faq/_index.md" >}}) zu achten!


#### 22.01.2021 Beitrag bei *This Week in Matrix (TWIM)*

Die Veröffentlichung der [Matrix Dokumentation auf GitHub](https://github.com/matrix-tu-dresden-de/Dokumentation) sowie die [Instanzkarte deutscher Hochschulen](https://doc.matrix.tu-dresden.de/why/) führten zu einer Einladung zu einem [Interview für *This Week in Matrix (TWIM)*](https://matrix.org/blog/2021/01/22/this-week-in-matrix-2021-01-22#superb-documentation-from-tu-dresden-as-they-roll-out-their-deployment). Hier stellten Marvin Dropp und Christian Bruchatz die Doku sowie die interaktive SVG der Instanzkarte vor und berichteten von den Matrix-Entwicklungen an der TU Dresden.

![TWIM-Interview 22.01.2021](/images/blog/04_TWIM-2021-01-22.png)

![TWIM-Interview 22.01.2021](/images/01_Find_de.png)


We set up a bilingual (de, en) documentation for all of our university members, to help them get in touch with our matrix instance easily. This documentation is rich on screenshots, simple explanations and will be improved continuously.

Also we mirroring the documentation to GitHub to provide access of our sources to everyone.



#### 22.01.2021 Instanzkarte

<object data="/images/federation_map.svg" type="image/svg+xml" style="width: 600px; max-width: 100%"></object>




Interaktive SVG



Aus Riot wird Element



Cross-Signing

https://jochen-plikat.com/2020/05/07/riot-cross-signing/

#### 04/2020 - Einführung von worker




#### 03/2020 - Stark ansteigende Nachfrage durch Corona {#firewall}



#### 01/2020 - Neustart des Servermonitorings {#firewall}



#### 01/2020 - Firewall-Freigabe für matrix.tu-dresden.de {#firewall}




#### 10/2019 - Pilotbetrieb unter matrix.tu-dresden.de beginn {#stable}

Nach Abschluss der 

Prof. Plikat spricht über die enorme Bedeutung von Matrix: https://jochen-plikat.com/2019/06/01/whatsapp-alternative-riot/




#### 04/2019 - CIO-Präsentation zu Empfehlungen von interner digitaler Kommunikation {#cio-vortrag}

Das [Team Impuls & Interaktion (TII)](https://tu-dresden.de/tu-dresden/profil/exzellenz/exzellenzinitiative-2012-2019/zukunftskonzept-1/zse/archiv) berät den CIO-Beirat der TU Dresden, mit welchen freien Tools eine Verbesserung der digitalen Infrastrukturen zur internen Kommunikation und Zusammenarbeit erzielt werden würde und wie den Wissenschaftler:innen an der TU Dresden dabei am meisten geholfen werden könnte. Als zentrales und wichtigstes Tool wird Matrix präsentiert. Die Unterstützung zahlreicher IT-Referenten bestätigte den eingeschlagenen Weg. Aufgrund mangelnder finanzieller Ressourcen wird eine Weiterentwicklung zwar nicht direkt unterstützt jedoch unter Selbstorganisation eines dezentralen Admin-Teams toleriert, dass unter der Schirmherrschaft vom Bereichs-CIO Mathematik und Naturwissenschaften, Prof. Dr. Oliver Sander, und unter Koordination des TIIs weiterarbeitet. Für eine geringfügige Fortführung der Arbeiten der studentischen Hilfskräfte sind der Professur für Softwaretechnologie und dem Team Impuls & Interaktion für ihre finanzielle Unterstützung zu danken.



#### 10/2018 - Matrix-Testserver geht online {#testserver}

Das [Team Impuls & Interaktion](https://tu-dresden.de/tu-dresden/profil/exzellenz/exzellenzinitiative-2012-2019/zukunftskonzept-1/zse/archiv) startet nach Tests mit [Mattermost](https://de.wikipedia.org/wiki/Mattermost), [Rocket.Chat](https://en.wikialpha.org/wiki/Rocket.chat) und [Zulip](https://en.wikipedia.org/wiki/Zulip) den ersten Matrix-Homeserver unter https://matrix.tii.tu-dresden.de und testet diesen mit interdisziplinären Communities aus der TU Dresden und ihren umliegenden Kooperationspartner:innen. Vielen Dank an Joris Baum für die initiale Installation sowie an die [Hochschulgruppe Freie Software Freies Wissen](https://fsfw-dresden.de/), insb. an Marcel Partap und Christoph Kleine, für die intensive Weiterentwicklung. Ein großer Dank gebührt auch dem [Zentrum für Informationsdienste und Hochleistungsrechnen (ZIH)](https://tu-dresden.de/zih/) sowie dem [Bereich Mathematik und Naturwissenschaften](https://tu-dresden.de/mn/der-bereich/leitung-und-verwaltung) für die finanzielle Unterstützung der ersten studentischen Hilfskräfte.



#### 06/2018 - Start der Planung{#start}

Im Zuge der Vorbereitung auf die zu erwartende digitale, asynchrone Zusammenarbeit im Exzellenzcluster *DCM - Dresden Center for Materiomics* begann das [Team Impuls & Interaktion](https://tu-dresden.de/tu-dresden/profil/exzellenz/exzellenzinitiative-2012-2019/zukunftskonzept-1/zse/archiv) mit der Konzipierung der zukünftigen internen Kommunikation.
