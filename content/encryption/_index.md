---
title: "Verschlüsselung"
date: 2020-07-03T13:20:58+02:00
draft: false
chapter: true
weight: 60
---

# Ende-zu-Ende-Verschlüsselung nutzen

1:1 Gespräche sind standardmäßig Ende-zu-Ende-verschlüsselt. Daher wird eine eingerichtete Schlüsselsicherung sowie eine Verifikation aller selbst eingesetzten Client-Geräte empfohlen (siehe [Wichtige Einstellungen]({{< ref "settings" >}})).

Die Entscheidung, ob ein erzeugter Raum verschlüsselt werden soll, muss gut überlegt sein und kann nicht mehr rückgängig gemacht werden. Wenn es sich um größere oder öffentliche Räume handelt, könnte das Prüfen aller Schlüssel aller Gesprächspartner viel Zeit in Anspruch nehmen. Diese manuelle Prüfung kann man aber auch später bei Gelegenheit durchführen und auch direkt Ende-zu-Ende-verschlüsselte Gespräche mit vorerst blindem Vertrauen starten.

![Neuen Raum mit aktivierter Verschlüsselung erstellen](/images/01_Create-Room-wE2E_de.png)

Wer in einem unverschlüsselten Raum eine Ende-zu-Ende-Verschlüsselung (E2EE) zu Gesprächspartner:innen wünscht, erreicht dies durch Klick auf die Einstellungen des gewünschten Raums. (bzw. im Raum über "Raum-Info" > "Raum-Einstellungen" oben rechts):

![Menü um zu den Raumeinstellungen zu gelangen](/images/02_Roomsettings_de.png)

Dazu ist im Reiter Sicherheit & Datenschutz der Schieberegler Verschlüsselt zu bewegen:

![Verschlüsselung in den Raumeinstellungen aktivieren](/images/03_Roome2e_de.png)

Dies kann mit OK bestätigt werden. Ab sofort können die Nachrichten nur noch von den am Gespräch Beteiligten gelesen werden. Sofern nicht schon vorab in den Einstellungen eine Schlüsselsicherung eingerichtet wurde, so sollte dies nun durchgeführt werden (siehe [Wichtige Einstellungen]({{< ref "settings" >}})), um frühere und in Abwesenheit empfangene Nachrichten lesen zu können.

Nun kann der verschlüsselte Austausch beginnen. Wenn man sich von der Korrektheit der Schlüssel überzeugen, und diese Vertrauenswürdigkeit digital dokumentieren möchte, ist dazu zuerst auf das Personensymbol oben rechts die Seitenleiste auszuklappen:

![öffnen der Personenliste in dem Raum](/images/04_RoomPeople_de.png)

In der sich öffnenden Leiste der am Gespräch Beteiligten kann nun auf die Kontaktperson geklickt werden:

![Raum mit Hinweis, dass nicht alle eilnehmenden verifiziert sind.](/images/05_People-Unverified_de.png)

Die Leiste zeigt jetzt die Gesprächsperson im Detail an. Hier ist eine Schlüsselverifikation durch Klick auf „Verifizieren“ einleitbar. Durch einen Klick auf "Starte Verifikation" wird die Gegenseiten benachrichtigt und nach Bestätigung (siehe nächstes Bild) kann die "Verifizierung durch Emojis" beginnen.

![Menü zu der zu verifizierenden Person mit dem Verifizieren-Knopf ausgewählt](/images/06_E2EE_Verify_de.png)

![Menü zum starten der Verifikation](/images/07_E2EE_Accept_de.png)

Diese Verifizierung sollte mit der Kontaktperson durch Abgleich (z.B. mündlichen via Telefon, im selben Zimmer oder anderes Medium) geschehen. Da dies nicht immer leicht ist, kann auch ersteinmal das Vertrauen ausgesprochen werden (sonst wird man immer wieder gefragt, die Verifizierung durchzuführen) und bei Gelegenheit (bspw. beim nächsten Meeting) durchzuführen.

Eine ausführliche Darstellung des Themas findet sich in diesem [Video von Prof. Plikat](https://invidious.ggc-project.de/VOxfa6dqXSk) sowie [im diesem Matrix-Blogartikel](https://blog.riot.im/e2e-encryption-by-default-cross-signing-is-here).

Der Abgleich selbst geschieht über Emoji-Bildchen oder QR-Codes, die je nach Gerät und Iconpack verschieden aussehen können. Auch ist die Übersetzung aller Oberflächenelemente ins Deutsche nicht 100%-ig vorhanden.

![Emojivergleich zum verifizieren des Schlüsselaustauschs](/images/16_E2EE.png)

Analog geschieht dies in Räumen mit mehreren Teilnehmenden, jeweils einzeln.

![Verifikationsprozess war erfolgreich](/images/08_Verified_de.png)

In den jeweiligen Raumzeilen deuten folgende Symbole den Status der Verschlüsselung und der dazugehörigen Verifikation an:

![Symbol für mindestens eine nicht-verifizierte Person](/images/gray.png)

Mindestens eine Person im Raum wurde noch nicht verifiziert.

![Symbol für eine verifizierte Person, die unverifizierte Sitzungen geöffnet hat](/images/unverified.png)

Im Raum ist mindestens eine Person, die bereits verifiziert wurde, aber die ihrerseits weitere unverifizierte Sitzungen geöffnet hat.

![Symbol für alle Personen im Raum sind verifiziert](/images/green.png)

Alle im Raum befindlichen Personen wurden verifiziert.

Hier ein weiteres Beispiel, wie man den Verschlüsselungszustand eines Raumes in den Rauminformationen oben rechts neben dem Raum-Icon erkennen kann:

![Darstellung der Verschlüsselungssituation in Matrix-Räumen](/images/room_security_status.png)


