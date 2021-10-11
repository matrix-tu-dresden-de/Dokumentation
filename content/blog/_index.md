---
menutitle: "Blog/News"
title: "Blog"
date: 2020-01-02T21:26:25+02:00
draft: false
weight: 200
---


***

#### 11.10.2021 Rauminhalte bequem exportieren {#export}

Seit Element-Version 1.9.1 ist es möglich, die Rauminhalte in einer .html, .txt oder .json Datei zu exportieren. 

![Export der Raumnachrichten](https://element.io/blog/content/images/size/w1000/2021/10/Screenshot-2021-10-11-at-10.21.21.png)

Vielen Dank an [Jaiwanth Vemula von der IIT Kharagpur University in Indien](https://element.io/blog/element-1-9-1-export-is-finally-here/)!


#### 08.10.2021 Spaces {#spaces}

Spaces heißt die Möglichkeit, Räume zu gruppieren und auch anderen Personen Zugriff auf viele Räume zu geben, sie bspw. in einen Space einzuladen, statt sie in viele Räume einzuladen.
Ideal für Studierende eines Jahrgangs, in deren Space sich alle Räume aller Lehrveranstaltungen befinden. Oder für Arbeitsgruppen, deren verschiedene Themenräume sich hier gebündelt vorfinden und neuen Teammitgliedern so schnell den Zugriff auf alle Räume bieten.
Spaces lösen die bisherigen Communities als Raumfilter ab.

https://element.io/blog/spaces-blast-out-of-beta/
https://element.io/blog/spaces-the-next-frontier/



#### 16.08.2021 Sprachnachrichten in Matrix/Element {#sprachnachrichten}

Seit Element-Version 1.8 sind [Sprachnachrichten](https://element.io/blog/introducing-voice-messages-and-so-much-more/) leicht einsprech- und absendbar.

![Sprachnachrichten](https://element.io/blog/content/images/2021/08/output-1.gif)


#### 27.07.2021 Deutsches Gesundheitswesen erhält Matrix Messenger

Das Deutsche Gesundheitsministerium verkündet die Einführung von Matrix als Messaging-Standard für das deutsche Gesundheitswesen ab 2022. Die [Gematik](https://fachportal.gematik.de/anwendungen/ti-messenger) benennt für diese Wahl vor allem folgende Gründe:
Das Open-Source-Messenger-Protokoll Matrix gewährleistet:
- Interoperabilität - und somit den sektoren- und anbieterübergreifenden Austausch
- Integrität dank hohem Out-of-the-box-Sicherheitsniveau,
- Ende-zu-Ende-Verschlüsselung sowie
- Innovation durch fortlaufende Weiterentwicklung.


Hochschulen-Artikel (Element), Uni Linz


#### 13.06.2021 TU Dresden hat mehr als 20.000 Matrix User {#20000}

Inzwischen hat wohl schon mehr als die Hälfte der TU Dresden Angehörigen Matrix ausprobiert. 


[![20.000 Matrix User @ TU Dresden](/images/blog/20210613_20000_Matrix_User.png)](https://doc.matrix.tu-dresden.de/Statistik/matrix-logins.html)

#### 28.04.2021 Relogin

Die TU Dresden taucht im [Element Blog](https://element.io/blog/universal-universities/) sowie einer [Element Education Sector Seite](https://element.io/sectors/education) als erfolgreiches Installations-Beispiel und mit der Instanzkarte auf.
Die [ETH Zürich](https://matrix.org/using-matrix/case-studies/eth-zurich-adopts-matrix-for-physics-department) berichtet darüber, wie mehr und mehr Teams von Slack zu Matrix wechseln.
Und die [Uni Innsbruch](https://element.io/case-studies/university-of-innsbruck) erklärt ausführlich ihren Weg zur Adoption von Matrix.


#### 27.03.2021 Relogin

Durch eine Aktualisierung am Matrix Server haben sich die Orte für Mediendateien verändert. Clients, die seit einem Zeitpunkt vor dem 28.03.2021 angemeldet sind, sehen Medien nicht mehr. Um dieses Problem zu lösen ist ein einmaliges Ab- und erneutes Anmelden nötig. Damit dabei keine früheren verschlüsselten Nachrichten unlesbar werden ist dringend auf die [in den FAQ beschriebene Prozedur]({{< relref "faq/_index.md" >}}) zu achten! Unsere großen Vorteile dadurch: Ab nun ist unser Matrix-Setup aber ein [MDAD](https://github.com/spantaleev/matrix-docker-ansible-deploy) mit automatischer Konfiguration der synapse worker und einer Verringerung der Angriffsgefahr durch Cross-Site Scripting (XSS).



#### 02.03.2021 Pull Request für MDAD synapse worker erfolgreich gemergt

Auf diesen Beitrag an der Matrix-Entwicklung kann die TU Dresden stolz sein! Am Wochenende wurde Pull Request (Vorschlag für verbesserten Programmcode) mit der Nummer [456](https://github.com/spantaleev/matrix-docker-ansible-deploy/pull/456) innerhalb des Matrix-Docker-Ansible-Deploy (MDAD) Repositoriums angenommen und in den Master-Zweig übernommen, der von der TU Dresden angestoßen und maßgeblich in den letzten 10 Monaten mitentwickelt wurde.
Die Code-Anpassungen, die den Dresdner Matrix-Dienst schon seit April 2020 für mittlerweile > 18.000 User stabil durch gezielte Lastverteilung auf sogenannte *synapse worker* ermöglichen, wurden durch mehrere Personen kollaborativ weiterentwickelt und stehen nun allen MDAD-Nutzenden weltweit frei zur Verfügung.
Die TU Dresden hat hier einmal mehr bewiesen, dass die Förderung von freier Software nicht nur durch die finanzielle Unterstützung einer Gruppe von Entwickelnden oder der direkten Beauftragung für die Entwicklung neuer Funktionen ([Beispiel LibreOffice](https://osb-alliance.de/pressemitteilungen/osb-alliance-meldet-erneut-erfolgreiches-crowdfunding-von-libreoffice-verbesserungen) oder [Beispiel PDF-Signaturen mit Okular](https://forums.puri.sm/t/okular-digital-signatures-and-tu-dresden/13808)) möglich ist. Wenn kaum Geld vorhanden ist, dann bleibt immerhin noch das Zurückspeisen von eigenen Weiterentwicklungen an die globale Community. 
Die Ausnutzung von synapse-worker durch Pull Request 456 versetzt andere große Institutionen (z.B. die vielen Hochschulen, die auch Matrix einsetzen) in die Lage eine stabile, skalierbare Instanz zu betreiben.


#### 22.01.2021 Beitrag bei *This Week in Matrix (TWIM)*

Die Veröffentlichung der zweisprachigen [Matrix Dokumentation auf GitHub](https://github.com/matrix-tu-dresden-de/Dokumentation) sowie die [Instanzkarte deutscher Hochschulen](https://doc.matrix.tu-dresden.de/why/) führten zu einer Einladung zu einem [Interview für *This Week in Matrix (TWIM)*](https://matrix.org/blog/2021/01/22/this-week-in-matrix-2021-01-22#superb-documentation-from-tu-dresden-as-they-roll-out-their-deployment). Hier stellten Marvin Dropp und Christian Bruchatz die Doku sowie die interaktive SVG der Instanzkarte vor und berichteten von den Matrix-Entwicklungen an der TU Dresden.

[![TWIM-Interview 22.01.2021](/images/blog/04_TWIM-2021-01-22.png)](https://inv.13ad.de/watch?v=UHJX2pmT2gk)

#### 22.01.2021 Instanzkarte

Uns bekannte Hochschulen und Universitäten mit einem Matrix-Dienst:

<object data="/images/federation_map.svg" type="image/svg+xml" style="width: 600px; max-width: 100%"></object>

#### 15.01.2021 Instanzkarte

Eine interaktive svg gibt einen Überblick über die Funktionalität und das Aussehen von Matrix/Element auf der Startseite der Dokumentation. Die Download-Links für Element sind so auch schnell erreichbar:

<object data="/images/matrix_interactive.svg" type="image/svg+xml" style="width: 1280px; max-width: 100%"></object>

#### 15.07.2020 Aus Riot wird Element

Der weniger geeignete Name *Riot* für den Referent-Client wird ad acta gelegt und mit Element bereichert sich die Matrix-Namenswelt der Firma New Vector Ltd. wieder im mathematischen Milieu. Passend auch für eine Technische Universität.

[1] https://element.io/blog/welcome-to-element/
[2] https://element.io/previously-riot


#### 01.07.2020 Intensivere Weiterentwicklung dank CIO-Unterstützung

Bisher finanzierten verschiedene Stellen der TUD verschiedene studentische Hilfskräfte, die das Matrix Setup der TU Dresden pflegen und weiterentwickeln. Seit Juli sind nun auch Mittel des CIO im Einsatz, was dem ganzen Projekt einen deutlichen Schub gibt und neuen SHK-Administrator:innen die Möglichkeit gibt, der TU Dresden an der Verbesserung ihrer Kommunikationsinfrastrukturen zu helfen!


#### 07.05.2020 Cross-Signing

Prof. Plikat erklärt fulminant das Cross-Signing zwischen verschiedenen Clients: https://jochen-plikat.com/2020/05/07/riot-cross-signing/



#### 06.04.2020 - Einführung von synapse workers

Wir nutzen [Matrix-Docker-Ansible-Deploy (MDAD)](https://github.com/spantaleev/matrix-docker-ansible-deploy), ein Geflecht von Ansible-Rollen für die verschiedenen Matrix-Dienste in Docker-Containern mit systemd-Steuerung. In diesem Framework ist ein Support für die experimentellen [synapse workers](https://github.com/matrix-org/synapse/blame/master/docs/workers.md) bisher noch von niemandem implementiert worden, es gibt dazu seit heute einen [Feature Request](https://github.com/spantaleev/matrix-docker-ansible-deploy/issues/221) von der TU Dresden. Diese Integration (also Anpassung der Ansible-Rollen) muss vorgenommen werden, so dass eine optimale Nutzung der Hardware (CPU-Kerne) gewährleistet und der TUD Matrix-Homeserver langfristig performant betrieben werden kann. Vielen Dank an Marcel Partap für die Arbeit an einem [Pull Request](https://github.com/spantaleev/matrix-docker-ansible-deploy/pull/456) und den parallelen manuellen Anpassungen hier an der TU Dresden, eine Entwicklung sozusagen am offenen Herzen...!


#### 03/2020 - Stark ansteigende Nachfrage durch Corona {#corona}



#### 01/2020 - Neustart des Servermonitorings {#servermonitoring}



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
