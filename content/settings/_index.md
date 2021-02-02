---
title: "Wichtige Einstellungen"
date: 2020-07-03T13:22:13+02:00
draft: false
chapter: true
weight: 10
---
# Empfehlungen zu Schritten nach dem Erstlogin

## Bequemes Nutzen der Ende-zu-Ende-Verschlüsselung (E2EE)

Matrix verschlüsselt nicht nur die Transporte von und zu dem Heimserver (im Rechenzentrum der TU Dresden) sondern erlaubt auch die Nutzung von Ende-zu-Ende-Verschlüsselung (E2EE). Hierzu müssen kryptografische Schlüssel zwischen allen Geräten ausgetauscht werden, die sich Ende-zu-Ende-verschlüsselt schreiben möchten. Diese technische Notwendigkeit klingt und ist kompliziert, ist inzwischen für die Anwendenden sehr bequem geworden. Die vielen kryptografischen Schlüssel werden vom Client erstellt auf dem jeweiligen Gerät gespeichert. Sollte dies bspw. ein Tab in einem Browser sein, besteht die Gefahr, dass dieser Tab einmal unbeabsichtigt geschlossen wird. Dann sind alle verschlüsselten Inhalte nicht mehr lesbar. Damit dies nicht geschieht, wird eine Schlüsselsicherung auf dem Heimserver der TU Dresden angeboten, auf der (mit einer Sicherheitsphrase (bzw. daraus errechenbaren Sicherheitsschlüssel) geschützt) alle kryptografischen Schlüssel verschlüsselt abgelegt sind. 

{{% notice warning %}}
Es wird dringend empfohlen, diese Schlüsselsicherung zu nutzen (mit einer sicheren Sicherheitsphrase, welche NICHT Ihr ZIH-Passwort ist) und am Punkt [Weitere wichtige Einstellungen]({{< relref "_index.md#weitere-wichtige-einstellungen" >}}) weiterlesen!
{{% /notice %}}
   
   ![Screenshot der Aufforderung eine Sicherheitsphrase einzugeben](/images/01_Restore-Session_de.png)

Sollten Sie dies jetzt überspringen, sähe der nächste Bildschirm so aus:
   
   ![Bestätigung des Überspringes der Eingabe einer Sicherheitsphrase](/images/03_Cancel-Restore_de.png)

Die Schlüsselsicherung wird dringend empfohlen, um sorgenfrei Ende-zu-Ende-Verschlüsselung nutzen zu können. Daher wird auch nach einem weiteren Überspringen in einem kleineren Tooltip zur Einrichtung der Verschlüsselung aufgefordert:
   
   ![Chatansicht mit der Anzeige eines Tooltips, Verschlüsselung einzurichten. Markierung des bestätigen Feldes](/images/04_Notification_de.png)

Sollten Sie dies auch hier auslassen wird Ihnen eine letzte Warnung bei einem bewussten Abmelden angezeigt. Wenn spätestens hierbei keine Schlüsselsicherung eingerichtet wird, kann später auf ggf. schon stattgefundene verschlüsselte Gespräche nicht mehr zugegriffen werden. Sollte der Tab geschlossen werden, entspricht dies ggf. ebenfalls einem Abmelden.
   
   ![Abfrage, ob Nachrichten verschlüsselt werden sollen](/images/05_Logout-Notify_de.png)

## Weitere wichtige Einstellungen

Nach erfolgreicher Einrichtung der Schlüsselsicherung aktivieren Sie nun die Desktop-Benachrichtigungen:
   
   ![Screenshot der Abfrage, Pushbenarchitigungen zu aktivieren](/images/06_Enable-Notifications_de.png)

   Dies kann später auch rückgängig gemacht werden und insb. können einzelne „Gespräche“ in ihrer Benachrichtigungsbefugnis eingestellt werden

Einstellungen im Einstellungsmenü vornehmen: dazu ist auf die Zeile der E-Mail-Adresse und des nach unten zeigenden Dreiecks zu klicken und anschließend auf die Zeile "Alle Einstellungen":

![Auswahl des Menüpunkts Einstellungen in dem Nutzer:innenmenü](/images/06_Settings_de.png)

In den Einstellungen können Sie im Reiter **Allgemein** bei Bedarf Ihren Anzeigenamen ändern („Vorname Nachname“) und ein Profilbild hochladen (analog zur Kontakbox auf der TUD-Website; Profilbild <5MB wählen):
![Makierung des Feldes Anzeigenamen und des Profilbilds in den Einstellungen](/images/06_Settings-Names_de.png)

Mittelfristig wird der Anzeigename aus dem Common Name im LDAP der TU Dresden erhalten, dann ist ein manuelles Ändern nicht mehr nötig.

Das E-Mail-Adressfeld ist nicht unbedingt zu füllen, da über Ihren ZIH-Login eine E-Mail-Adresse hinterlegt ist. Theoretisch können hier weitere Adressen hinzugefügt werden, bspw. um Benachrichtigungen über verpasste Nachrichten an eine weitere E-Mail-Adresse senden zu lassen.

Auf der selben Seite kann auch das Design Thema von hell zu dunkel verändert werden.

Im Reiter **Benachrichtigungen** können Sie E-Mail-Benachrichtigungen (um über verpasste Nachrichten informiert zu werden) sowie akustische Benachrichtigungen aktivieren und diese granular für einzelne Aktivitäten Anderer einstellen. Mehr dazu auf der Seite [Benachrichtigungen]({{< relref "notifications" >}}).

![Screenshot der Benarchrichtigungeneinstellungen mit einer Makierung der ausgeschalteten E-Mail benachrichtigungen](/images/06_Settings-EMailNotify_de.png)

Im Reiter **Sprache & Video** können Sie den Matrix-Client Element berechtigen Ihre Medien (Kamera + Mikrofon) zu nutzen, direkten Sprach-/Videoanrufe mittels Peer-to-Peer-Verbindungen erlauben, sowie bei Videotelefonaten sich selbst in einem kleinen Bild zu sehen:

![Screenshot des Einstellungsmenüs Sprache und Video](/images/06_Settings-Media_de.png)

Erfreulicherweise starten 1:1 Gespräche standardmäßig Ende-zu-Ende-verschlüsselt. Um dieser Verschlüsselung wirklich mit gutem Gefühl zu vertrauen, können Nutzer:innen den Schlüsselvergleich mit Gesprächspartner:innen durchführen. Damit dies dann auch für alle Geräte dieser Gesprächspartner:innen gilt, müssen Matrix-Nutzenden ihrerseits wiederum die Schlüssel all ihrer Geräte untereinander verifizieren (Fachbegriff: Cross-Signing). Unter Beachtung der nachfolgenden Hinweise kann dies alles sehr bequem geschehen.

## Sicherheit & Datenschutz
Im Reiter **Sicherheit & Datenschutz** finden Sie alle Ihre Geräte, die bisher vom Matrix-Account genutzt wurden. 

* Entfernen Sie ggf. nicht mehr benutzte Sitzungen durch Markierung der quadratischen Box am Zeilenende und dem Klick auf den sich dann zeigenden roten Button.
  
![Screenshot des Menüs zum löschen von aktiven Sessions](/images/09_Delete-Sessions_de.png)

* Die Geräte-Namen geben Ihnen auch Übersicht beim gegenseitigen Schlüsselvergleich zwischen Ihren Geräten. 

* Die hier vergebbaren öffentlichen Namen (durch Mausklick auf diese) Ihrer Geräte können auch von Gesprächspartner:innen eingesehen werden.  Dies hilft, wenn diese einen Vergleich der kryptografischen Schlüssel Ihrer Geräte (bspw. Laptop + Handy) durchzuführen möchten und so leicht die Gerätenamen identifizieren können.

* Die vielen kryptografischen Schlüssel werden auf dem jeweiligen Gerät gespeichert. Sollte dies bspw. ein Tab in einem Browser sein, besteht die Gefahr, dass dieser Tab einmal unbeabsichtigt geschlossen wird. Dann sind alle verschlüsselten Inhalte nicht mehr lesbar. Damit dies nicht geschieht, wird eine Schlüsselsicherung auf dem Heimserver der TU Dresden angeboten, auf der (mit einer Passphrase geschützt) alle kryptografischen Schlüssel verschlüsselt abgelegt sind. Es wird dringend empfohlen, diese Schlüsselsicherung zu nutzen!

![Screenshot des Menüpunkts zur Schlüsselsicherung](/images/10_Setup-Keystore_de.png)

## Schlüsselsicherung 
Sofern nicht nach Erstanmeldung eingerichtet: Die **Schlüsselsicherung** ist eine wertvolle Errungenschaft, da Sie ermöglicht, die Schlüssel aller Gespräche, die Ende-zu-Ende-verschlüsselt sind, mit einem Passwort versehen zentral auf dem Server der TU Dresden zu sichern. Dies ermöglicht bequem die Nutzung mehrerer Geräte bzw. Matrix-Clients. Hierzu ist auf „Beginne Schlüsselsicherung zu nutzen“ zu klicken und eine starke Sicherheitsphrase (aber nicht das ZIH-Passwort) zu wählen. Diese Sicherheitsphrase wird immer einzugeben sein, wenn Schlüssel mit der Schlüsselsicherung synchronisiert werden sollen.

![Aufforderung den Sicherheitsschlüssel zu generieren oder eine Sicherheitsphrase einzugeben](/images/11_Setup-Key_de.png)
![Aufforderung eine Passwort für die Schlüsselsicherung einzugeben](/images/12_Enter-Key_de.png)
Alternativ können Sie sich statt der Sicherheitsphrase auch einen Sicherheitsschlüssel generieren lassen, welcher den selben Zweck wie die Sicherheitsphrase erfüllt. Weiterhin wird der Sicherheitsschlüssel zusätzlich zur Sicherheitsphrase erstellt und sollte als Notfallschlüssel sicher und wiederauffindbar verwahrt werden (z.B. Abspeichern als .txt-Datei oder Ausdrucken) 
![Anzeige des Sicherheitsschlüssel zum abschreiben oder wegspeichern](/images/13_Present-Key_de.png) 
