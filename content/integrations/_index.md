---
title: "Integrationen"
date: 2020-07-02T21:23:01+02:00
draft: false
chapter: true
weight: 80
---

# Integrations, Bridges, Bots nutzen (u.a. Jitsi)

Über die Rauminformationen oben rechts können [Integrations]/(https://matrix.org/docs/guides/types-of-bridging) / Widgets verwaltet werden.

![Integration hinzufügen button](/images/01_Widgets_de.png)

Hier kann bspw. ein Etherpad, eine Jitsi-Videokonferenz, ein RSS-Bot o.a. eingebunden werden, also Dienste, die auf anderen Servern liegen und ausgeführt werden. Daher ist bei Nutzung von Integrations auch die JavaScript-Aktivität von vector.im (für den Integrationsmanager) und weiteren Servern (bspw. im Firefox-Addon NoScript) zu erlauben. Da die Widgets oftmals zu klein sind, um die Dienste in ihrer vollen Funktionalität zu nutzen, lassen sich Widgets auch oft in neuen Browser-Tabs groß öffnen.

Prof. Dr. Alexander Lasch präsentiert in folgenden Videos einige Möglichkeiten zum Einbinden von Widgets in Matrix-Räume für die digitale Lehre:

https://invidious.13ad.de/watch?v=AtkA-sE-9uU

https://invidious.13ad.de/watch?v=D2Pq-NCaVGE

## Jitsi Videokonferenz

Ein 1:1 Telefonat oder Video innerhalb von Matrix nutzt die direkte WebRTC-Verbindung zwischen beiden Beteiligten. Ab der 3. Person wird [Jitsi](https://de.wikipedia.org/wiki/Jitsi) hinzugezogen, ein freies Videokonferenz-Tool (Apache-Lizenz), welches im Zuge der Corona-Krise und der verminderten Verfügbarkeit vom DFNconf auch lokal an der TU Dresden installiert wurde: https://jitsi.tu-dresden.de

Wenn das Videotelefonat über das Kameraicon rechts unten begonnen wird, wird automatisch das von der TU Dresden betriebene Jitsi verwendet. Damit Jitsi für die Videokonferenz verwendet wird, müssen mindestens drei Personen an der Konferenz teilnehmen. Wenn nur zwei Personen an der Konferenz teilnehmen, wird eine Direktverbindung aufgebaut.

{{% notice warning %}}
Wenn die Jitsi-Integration über den Integrationmanager hinzugefügt wird, wird nicht die Jitsiinstanz der TU Dresden verwendet
{{% /notice %}}

Auch bei Jitsi ist das öffnen des Widgets als eigener Tab sinnvoll, um die volle Funktionalität (bspw. Bildschirm teilen / Screensharing) zu nutzen. 

Die Nutzung eines Headsets (Kopfhörer + Mikrofon) ist sehr zu empfehlen, um Rückkopplungen zwischen Tonaufnahme und Tonwiedergabe zu verhindern. Idealerweise ein Headset mit Mikro in Kopfnähe und nicht nur ein Kopfhörer und eine Nutzung des Mikro-Löchleins am Laptop, was zu Geräuschen durch diesen führt.

Die Taste m schaltet das eigene Mikrofon stumm - mit dieser Einstellung sollte man immer in eine Konferenz starten. Die Leertaste schaltet bei aktiver Stummschaltung das Mikrofon an (Push-to-talk). Da die Mikrofon-Eingangspegel alle unterschiedlich einstellen, können alle hörenden Teilnehmenden die Lautstärke aller Konferenzteilnehmenden individuell anpassen. Weiterhin ist die eigene Videoqualität einstellbar. 

Für das Teilen des Bildschirminhaltes (bzw. spezifischer Programmfenster) ist ggf. eine Anpassung der Sicherheitseinstellungen des Betriebssystems nötig (bspw. in MacOS unter Systemeinstellungen > Sicherheit > Datenschutz > Bildschirmaufnahme).

Vielen Dank an Dr. Eike Dohmen ([Professur für Magnetofluiddynamik, Mess- und Automatisierungstechnik](https://tu-dresden.de/ing/maschinenwesen/imd/mfd)) und Prof. Dr. Alexander Lasch ([Professur für Germanistische Linguistik und Sprachgeschichte](http://tu-dresden.de/gsw/slk/germanistik/gls/)) für Tests und Hinweise zum Zusammenspiel von Matrix und Jitsi.

## Etherpad

Zum kollaborativen Schreiben oder Anheften von wichtigen Informationen an einen Raum kann das Widget Etherpad genutzt werden.

{{% notice warning %}}
Hierzu ist ein Name zu vergeben, der weniger als 16 Zeichen haben muss!
{{% /notice %}}
Etherpads haben kein Benutzerrechtemanagement, alle können schreiben und andere Texte überschreiben (Vorsicht!). Falls Benutzermanagement benötigt wird besser [Nextcloud Text](https://github.com/nextcloud/text) (Forderung an TUD cloudstore richten) oder [CodiMD](https://md.inf.tu-dresden.de/) nutzen

## Element Matrix Services (EMS) bieten Bridge für Microsoft Teams an

Um Benutzende von Element und MS Teams zusammenzubringen bietet EMS eine MS Teams Bridge an, die allerdings kostenpflichtig ist:
[https://element.io/blog/ems-launches-bridging-for-microsoft-teams/](https://element.io/blog/ems-launches-bridging-for-microsoft-teams/) und [https://element.io/blog/microsoft-teams-and-slack-integration-using-matrix/](https://element.io/blog/ems-launches-bridging-for-microsoft-teams/).

## Custom Widget

Hierbei können beliebige Internetseiten eingebunden werden. Bspw. [CodiMD](https://md.inf.tu-dresden.de/), um LaTeX-Formeln anzuzeigen.


