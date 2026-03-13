---
title: "Communities"
date: 2020-07-02T21:22:34+02:00
draft: false
chapter: true
weight: 50
---

# Communities (veraltet)

{{% notice note %}}
[Spaces]({{< relref "spaces/_index.md" >}}) lösen die Communities zur Raumverwaltung ab. Die Funktion ist in aktuellen Element-Versionen automatisch aktiviert. <!--(Desktop/Web 1.9, Android 1.3, iPadOS/iOS 1.6 oder neuer)-->
{{% /notice %}}

## Inhalt
  * [Communities temporär anzeigen](#communities-temporär-anzeigen)
  * [Communities konvertieren](#communities-konvertieren)
  * [Communities als Raum-Filter einsetzen](#communities-als-raum-filter-einsetzen)

## Communities temporär anzeigen

![Auswahl des Punkts "Alle Einstellungen" im personlichen Menü](/images/06_Settings_de.png)

Klicken Sie auf den nach unten zeigenden Pfeil oben rechts in der Personenspalte und rufen Sie `Alle Einstellungen` auf.

![Element-Einstellungen mit Optionen zu Communities](/images/20_Communities_Settings1_de.png)

Wählen Sie im Dialog links den Punkt `Optionen` (1) aus. Auf der Rechten Seite finden Sie unter der Überschrift `Communities` die Option `Communities statt Spaces anzeigen` (2). Aktivieren Sie den Regler rechts daneben, wird Ihr Element-Client neu geladen und die Communities werden angezeigt. Klicken Sie erneut auf den Regler, wenn Sie zur regulären Ansicht zurückkehren möchten.

## Communities konvertieren

![Auswahl des Punkts "Alle Einstellungen" im personlichen Menü](/images/06_Settings_de.png)

Klicken Sie auf den nach unten zeigenden Pfeil oben rechts in der Personenspalte und rufen Sie `Alle Einstellungen` auf.

![Element-Einstellungen mit Optionen zu Communities](/images/20_Communities_Settings2_de.png)

Wählen Sie im Dialog links den Punkt `Optionen` (1) aus. Auf der Rechten Seite finden Sie unter der Überschrift `Communities` den Eintrag `Meine Communities anzeigen` (2). Klappen Sie den Eintrag aus, werden Ihre Communities angezeigt. Mit einem Klick auf den Button `Space erstellen` (3) jeweils rechts neben einem Eintrag wird der Konvertierungsdialog aufgerufen.

![Dialog für die Konvertierung einer Community zu einem Space](/images/20_Communities_Conversion1_de.png)

Hier können Sie den das Foto, den Namen, die Beschreibung und die Sichtbarkeit (privat oder öffentlich) des Spaces konfigurieren. Anschließend kann die Konvertierung mit einem Klick auf `Space erstellen` gestartet werden.

![Dialog mit Erfolsmeldung nach der Konvertierung](/images/20_Communities_Conversion2_de.png)

Ist der Prozess abgeschlossen, erhalten Sie eine Erfolgsmeldung. Über den Button `Optionen` gelangen Sie wieder in die Einstellungen für Communities.

## Communities als Raum-Filter einsetzen

Alle Matrix-Nutzenden des Clients Element (und einiger weniger weiterer Clients) können Communities (zu deutsch Gemeinschaften) nutzen, um verschiedene Räume zu filtern, die in der Raumliste links vllt. untergehen oder zu verstreut platziert sind.

Communities können nur für sich selbst oder für Andere erstellt werden (wenn man diese in eine Community einlädt) und schaffen eine übergeordnete Struktur für Räume. Beispielsweise für eine Semestergruppe/Studiengruppe oder für ein Lehrstuhlteam etc.

Bestehende Räume können einer Community in den Community-Einstellungen zugewiesen werden.

![Screenshot der Auswahl der aktuellen Community](/images/20_Communities.webp)

Eine über den + Knopf erstellte Community kann per Drag'n'Drop des Community-Avatares (Bildchens) auf die Seitenleiste gezogen werden.

Eine kleine HTML-Seite kann zur Communitybeschreibung benutzt werden.

Leider ist derzeit das hinzufügen von weiteren Administratoren durch den Matrixclient nicht möglich: [https://github.com/vector-im/element-web/issues/5240](https://github.com/vector-im/element-web/issues/5240)

Das Entfernen von Räumen aus Communities geht durch Klick auf die Raute # oben rechts, einem anschließenden Klick auf den zu entfernenden Raum und dann dem Klick auf „Aus der Community entfernen“.

Eine Community kann gelöscht werden, wenn die administrierende Person diese verlässt.

<!--
### weitere Administratoren

Über Element können aktuell keine weiteren Administratoren zu einer Community hinzugefügt werden. [Issue auf Github](https://github.com/vector-im/riot-web/issues/5240) Wenn Sie weitere Administratoren in einer Community benötigen, können diese durch das Matrix Admin Team hinzugefügt werden. Schreiben Sie dazu bitte eine Supportanfrage an servicedesk@tu-dresden.de.
-->
