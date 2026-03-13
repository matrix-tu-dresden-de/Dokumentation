---
title: "Integrationen"
date: 2020-07-02T21:23:01+02:00
draft: false
chapter: true
weight: 80
---

# Integrationen

Integrationen erweitern den Funktionsumfang von Matrix.

* [Verwaltung](#management)
* [Widgets](#widgets)
  * [Jitsi (Videokonferenz)](#jitsi)
  * [Etherpad (Texteditor)](#etherpad)
  * [Custom Widget](#custom-widget)
* [Bots](#bots)
* [Bridges](#bridges)
  * [Microsoft Teams](#microsoft-teams)

## Verwaltung {#management}

In Element können über die Rauminfo Integrationen verwaltet werden. Der entsprechende Button findet sich am Ende der obersten Zeile eines Raumes.

![Erklärender Screenshot zur vorangegangen Beschreibung mit Markern auf dem Rauminfo-Button und dem Button zum Hinzufügen von Widgets, Bridgets und Bots](/images/01_Widgets_de.png)

Hier kann bspw. ein Etherpad, eine Jitsi-Videokonferenz, ein RSS-Bot o.a. eingebunden werden, also Dienste, die auf anderen Servern liegen und ausgeführt werden. Daher ist bei Nutzung von Integrations auch die JavaScript-Aktivität von vector.im (für den Integrationsmanager) und weiteren Servern (bspw. im Firefox-Addon NoScript) zu erlauben. Da die Widgets oftmals zu klein sind, um die Dienste in ihrer vollen Funktionalität zu nutzen, lassen sich Widgets auch oft in neuen Browser-Tabs groß öffnen.

## Widgets

Widgets betten Apps in Räume ein, sodass dessen Mitglieder gemeinsam darauf zugreifen können.

{{% notice warning %}}
Die TU Dresden stellt mit Matrix lediglich eine Plattform zur Verfügung. Bei der Einbindung von Widgets werden gegebenenfalls personenbezogenen Daten an Dritte übermittelt. Die Verantwortlichkeit dafür liegt bei den Nutzer:innen, zwischen denen und den Drittparteien die Übermittlung dieser Daten direkt erfolgt.
{{% /notice %}}

Prof. Dr. Alexander Lasch präsentiert in folgenden Videos einige Möglichkeiten zum Einbinden von Widgets in Matrix-Räume für die digitale Lehre:

* [Digitale Lehre 1: MATRIX Web Messenger](https://youtube.de/watch?v=AtkA-sE-9uU)
* [Digitale Lehre 5: Videokonferenz via Jitsi @ MATRIX](https://youtube.de/watch?v=D2Pq-NCaVGE)

### Jitsi (Videokonferenz) {#jitsi}

{{% notice tip %}}
Wird ein Video- oder Sprachanruf über die entsprechenden Buttons im Raum mit mehr als zwei Personen gestartet, wird Jitsi auf den Servern der TU Dresden verwendet.
{{% /notice %}}


<!-- Ein 1:1 Telefonat oder Video innerhalb von Matrix nutzt die direkte WebRTC-Verbindung zwischen beiden Beteiligten. Ab der 3. Person wird [Jitsi](https://de.wikipedia.org/wiki/Jitsi) hinzugezogen, ein freies Videokonferenz-Tool (Apache-Lizenz), welches im Zuge der Corona-Krise und der verminderten Verfügbarkeit vom DFNconf auch lokal an der TU Dresden installiert wurde: https://jitsi.tu-dresden.de

Wenn das Videotelefonat über das Kameraicon rechts unten begonnen wird, wird automatisch das von der TU Dresden betriebene Jitsi verwendet. Damit Jitsi für die Videokonferenz verwendet wird, müssen mindestens drei Personen an der Konferenz teilnehmen. Wenn nur zwei Personen an der Konferenz teilnehmen, wird eine Direktverbindung aufgebaut.

{{% notice warning %}}
Wenn die Jitsi-Integration über den Integrationmanager hinzugefügt wird, wird nicht die Jitsiinstanz der TU Dresden verwendet
{{% /notice %}} -->

Auch bei Jitsi ist das öffnen des Widgets als eigener Tab sinnvoll, um die volle Funktionalität (bspw. Bildschirm teilen / Screensharing) zu nutzen.

Die Nutzung eines Headsets (Kopfhörer + Mikrofon) ist sehr zu empfehlen, um Rückkopplungen zwischen Tonaufnahme und Tonwiedergabe zu verhindern. Idealerweise ein Headset mit Mikro in Kopfnähe und nicht nur ein Kopfhörer und eine Nutzung des Mikro-Löchleins am Laptop, was zu Geräuschen durch diesen führt.

Die Taste m schaltet das eigene Mikrofon stumm - mit dieser Einstellung sollte mensch immer in eine Konferenz starten. Die Leertaste schaltet bei aktiver Stummschaltung das Mikrofon an (Push-to-talk). Da die Mikrofon-Eingangspegel alle unterschiedlich einstellen, können alle hörenden Teilnehmenden die Lautstärke aller Konferenzteilnehmenden individuell anpassen. Weiterhin ist die eigene Videoqualität einstellbar.

Für das Teilen des Bildschirminhaltes (bzw. spezifischer Programmfenster) ist ggf. eine Anpassung der Sicherheitseinstellungen des Betriebssystems nötig (bspw. in MacOS unter Systemeinstellungen > Sicherheit > Datenschutz > Bildschirmaufnahme).

Vielen Dank an Dr. Eike Dohmen ([Professur für Magnetofluiddynamik, Mess- und Automatisierungstechnik](https://tu-dresden.de/ing/maschinenwesen/imd/mfd)) und Prof. Dr. Alexander Lasch ([Professur für Germanistische Linguistik und Sprachgeschichte](http://tu-dresden.de/gsw/slk/germanistik/gls/)) für Tests und Hinweise zum Zusammenspiel von Matrix und Jitsi.

### Etherpad (Texteditor) {#etherpad}

Zum kollaborativen Schreiben oder Anheften von wichtigen Informationen an einen Raum kann das Widget Etherpad genutzt werden.

{{% notice warning %}}
Hierzu ist ein Name zu vergeben, der weniger als 16 Zeichen haben muss!
{{% /notice %}}
Etherpads haben kein Rechtemanagement, alle können schreiben und andere Texte überschreiben (Vorsicht!). <!-- Falls ein Rechtemanagement benötigt wird besser [Nextcloud Text](https://github.com/nextcloud/text) (Forderung an TUD cloudstore richten) nutzen. -->

### Custom Widget

Hierbei können beliebige Internetseiten eingebunden werden.

## Bots

Bots sind Matrix-Konten, die in Räumen auf Befehle reagieren.

## Bridges

Bridges stellen eine Verbindung mit einem anderen Dienst her, sodass aus Matrix heraus mit Nutzer:innen anderer Chat-Dienste kommuniziert werden kann.

<!-- [Bridges](https://matrix.org/docs/guides/types-of-bridging) -->

### Microsoft Teams

Um Nutzer:innen von Element und MS Teams zusammenzubringen, bietet Element Matrix Services (EMS) eine MS Teams Bridge an, die allerdings kostenpflichtig ist. Siehe:
* [element.io/blog/ems-launches-bridging-for-microsoft-teams/](https://element.io/blog/ems-launches-bridging-for-microsoft-teams/)
* [element.io/blog/microsoft-teams-and-slack-integration-using-matrix/](https://element.io/blog/ems-launches-bridging-for-microsoft-teams/)
