---
title: "Wichtige Einstellungen"
date: 2020-07-03T13:22:13+02:00
draft: false
chapter: true
weight: 10
---

# Einstellungen nach dem ersten Login

## Aktivieren der Desktop-Benachrichtigungen

Ähnlich zu der Einrichtung der Schlüsselsicherung werden Sie nach der Anmeldung irgendwann dazu aufgefordert die Desktop-Benachrichtigungen zu aktivieren.
Dies kann später geändert oder rückgängig gemacht werden. Insbesondere können die Benachrichtigungen für einzelne "Gespräche" (Räume) individuell eingestellt werden.

![Screenshot der Abfrage, Pushbenarchitigungen zu aktivieren](/images/06_Enable-Notifications_de.png)

## Öffnen der Einstellungen

Das **Einstellungsmenü** kann geöffnet werden indem auf das runde Anzeigebild oben Links und anschließend auf die Zeile "Alle Einstellungen" geklickt wird.

![Auswahl des Menüpunkts Einstellungen in dem Nutzer:innenmenü](/images/06_Settings_de.png)

## Anzeigename und Profilbild

In den Einstellungen können Sie im Reiter **Account** bei Bedarf Ihren Anzeigenamen ändern („Vorname Nachname“) und ein Profilbild hochladen (analog zur Kontakbox auf der TUD-Website; Profilbild <5MB wählen):
![Markierung des Feldes Anzeigenamen und des Profilbilds in den Einstellungen](/images/06_Settings-Names_de.png)

Mittelfristig wird der Anzeigename aus dem Common Name im LDAP der TU Dresden erhalten, dann ist ein manuelles Ändern nicht mehr nötig.

Das E-Mail-Adressfeld sollte nicht ausgefüllt werden, da über Ihren TUB-Login eine E-Mail-Adresse hinterlegt ist. Theoretisch können hier weitere Adressen hinzugefügt werden, beispielsweise um Benachrichtigungen über verpasste Nachrichten an eine weitere E-Mail-Adresse senden zu lassen.

## Erscheinungsbild

Auf dieser Seite kann das Design Thema von hell zu dunkel verändert oder die Schriftgröße angepasst werden.

## Benachrichtigungen

Im Reiter **Benachrichtigungen** können Sie E-Mail-Benachrichtigungen (um über verpasste Nachrichten informiert zu werden) sowie akustische Benachrichtigungen aktivieren und diese granular für einzelne "Gespräche" (Räume) einstellen. Mehr dazu auf der Seite [Benachrichtigungen]({{< relref "notifications" >}}).

![Screenshot der Benarchrichtigungeneinstellungen mit einer Makierung der ausgeschalteten E-Mail benachrichtigungen](/images/06_Settings-EMailNotify_de.png)

## Allgemeine Einstellungen

Im Reiter **Einstellungen** finden Sie eine Vielzahl verschiedener Optionen, um den Matrix Client an Ihre Bedürfnisse anzupassen. So können Tastenkombinationen festgelegt werden, die Nachrichteneingabe angepasst werden oder aber auch Lesebestätigungen von Nachrichten deaktiviert werden.

## Telefonie

Im Reiter **Anrufe** können Sie den Matrix-Client Element berechtigen Ihre Mediengeräte (Kamera + Mikrofon) zu nutzen sowie Sprach-/Videoanrufe mittels direkter Peer-to-Peer-Verbindungen erlauben:

![Screenshot des Einstellungsmenüs Sprache und Video](/images/06_Settings-Media_de.png)

Erfreulicherweise starten 1:1 Gespräche standardmäßig Ende-zu-Ende-verschlüsselt. Um dieser Verschlüsselung wirklich mit gutem Gefühl zu vertrauen, können Nutzer:innen den Schlüsselvergleich mit Gesprächspartner:innen durchführen. Damit dies dann auch für alle Geräte dieser Gesprächspartner:innen gilt, müssen Matrix-Nutzenden ihrerseits wiederum die Schlüssel all ihrer Geräte untereinander verifizieren (Fachbegriff: Cross-Signing). Unter Beachtung der nachfolgenden Hinweise kann dies alles sehr bequem geschehen.

## Sicherheit & Datenschutz

Im Reiter **Sitzungen** finden Sie alle Ihre Geräte, die bisher vom Matrix-Account genutzt wurden.

Entfernen Sie ggf. nicht mehr benutzte Sitzungen durch Markierung der quadratischen Box am Zeilenende und dem Klick auf den sich dann zeigenden roten Button.

![Screenshot des Menüs zum löschen von aktiven Sessions](/images/09_Delete-Sessions_de.png)

Die Geräte-Namen geben Ihnen auch Übersicht beim gegenseitigen Schlüsselvergleich zwischen Ihren Geräten.

Die hier vergebbaren öffentlichen Namen (durch Mausklick auf diese) Ihrer Geräte können auch von Gesprächspartner:innen eingesehen werden. Dies hilft, wenn diese einen Vergleich der kryptografischen Schlüssel Ihrer Geräte (bspw. Laptop + Handy) durchzuführen möchten und so leicht die Gerätenamen identifizieren können.

Die vielen kryptografischen Schlüssel werden auf dem jeweiligen Gerät gespeichert. Sollte dies bspw. ein Tab in einem Browser sein, besteht die Gefahr, dass dieser Tab einmal unbeabsichtigt geschlossen wird. Dann sind alle verschlüsselten Inhalte nicht mehr lesbar. Damit dies nicht geschieht, wird eine Schlüsselsicherung auf dem Heimserver der TU Dresden angeboten, auf der (mit einer Passphrase geschützt) alle kryptografischen Schlüssel verschlüsselt abgelegt sind. Es wird dringend empfohlen, diese Schlüsselsicherung zu nutzen!

<!--![Screenshot des Menüpunkts zur Schlüsselsicherung](/images/10_Setup-Keystore_de.png)-->

## Einrichtung der Schlüsselsicherung

Sollten Sie nach der ersten Anmeldung nicht automatisch dazu aufgefordert worden sein die Schlüsselsicherung einzurichten, empfiehlt es sich die Schlüsselsicherung jetzt einzurichten. Das ist in den Einstellungen im Reiter **Sicherheit** möglich. Weitere Informationen finden Sie in unter [Erste Schritte]({{< relref "first-steps/_index.md#einrichtung-der-schlüsselsicherung" >}}).
