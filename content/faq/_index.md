---
menutitle: "Häufige Fragen (FAQ)"
title: "Häufig gestellte Fragen"
date: 2020-08-02T21:26:25+02:00
draft: false
weight: 200
---

Dies ist eine Zusammenstellung häufiger Fragen und deren Antworten. Unbeantwortete Fragen können Sie gerne im Raum `#matrix-support:tu-dresden.de` stellen.

## Inhaltsverzeichnis

### Schlüsselsicherung

* [Warum sind meine Nachrichten nicht lesbar?](#unable-to-decrypt)
* [Ich habe Schwierigkeiten beim Verifizieren einer neuen Sitzung](#verify-client)
* [Warum muss ich meinen Sicherheitsschlüssel speichern?](#store-securitykey)
* [Was ist der Unterschied zwischen einem Sicherheitsschlüssel und einer Sicherheitsphrase?](#securitykey-vs-securityphrase)
* [Wie ändere ich die Sicherheitsphrase für meine Schlüsselsicherung?](#change-securityphrase)
* [Wie kann ich die Schlüsselsicherung zurücksetzen, wenn ich meine Sicherheitsphrase UND meinen Sicherheitsschlüssel verloren habe?](#reset-securityphrase)

### Allgemeines

* [Wie teilt man Leuten mit dem Element-Client eine Raumadresse mit?](#share-room)
* [Wie kann man in einer Gruppe, in der sich der einzige Admin entfernt hat, wieder einen Admin neu definieren?](#no-admin)
* [Kann ich LaTeX schreiben?](#latex)
* [Gibt es sowas wie Threads (vgl. Mattermost/Slack) in Matrix?](#threads)
* [Warum gibt es keinen Raum "TU Dresden"? Wer dürfte ihn erstellen?](#no-tud-room) <!--* [Wie kann ich als administrierende Person viele Nachrichten auf einmal löschen?](#delete-multiple-messages)-->
* [Ich kann mich über die Element IOS-App nicht anmelden](#apple-anmeldung)
* [Was muss ich tun, wenn auf einem MacOS Video oder Audio in einer Videokonferenz nicht funktioniert?](#apple-no-video)
* [Wie viele Personen können gleichzeitig in einen Raum eingeladen werden? Kann ich Personen über ihre E-Mail-Adressen einladen?](#how-many-invites-can-i-do)<!--* [Kann ich die Beitrittsrechte aller Räume meiner Community so anpassen, dass nur Mitglieder der Community Zutritt haben?](#roompermissions-in-communities)-->
* [Kann ich mit Element mehrere Matrix-Accounts verwalten (Multi-Account-Client)?](#multiple-accounts-element)
* [Überall steht nur „missing translation: en“](#missing-translations)
* [Ist unser Server auf eurer Föderations-Blacklist?](#blacklist)
* [Ich sehe in einem Raum von einer bestimmten Person keine Nachrichten](#blocked-user)
* [Warum sieht man im Element Desktop-Client keine Statuszeile am unteren Ende des Bildschirms wenn man die Maus über Hyperlinks bewegt?](#no-statusline)

***
### Schlüsselsicherung

#### Warum sind meine Nachrichten nicht lesbar? {#unable-to-decrypt}
* Der Matrix-Client kann die Nachrichten nicht entschlüsseln, weil die persönlichen Schlüssel nicht abrufbar sind.
* Damit die Entschlüsselung ordnungsgemäß funktioniert, muss die [Schlüsselsicherung]({{< relref "first-steps/#einrichtung-der-schlüsselsicherung" >}}) eingerichtet sein.
* Wenn eine alte Matrix-Sitzungen ohne Abmeldung geschlossen wurde, sodass kein Zugriff auf diese Sitzungen mehr besteht (z.B. Browser-Tab geschlossen, Element-Installation auf altem Rechner), dann kann es passieren, dass Nachrichten aus dieser Sitzung nicht entschlüsselt werden können. Die alten Sitzungen sollten in den Einstellungen unter "Sitzungen" entfernt werden.
* Es sollte immer mindestens eine verifizierte Sitzung aktiv sein. Am besten ist es, wenn der Desktop Client oder Element auf dem Smartphone eingerichtet ist. Diese Apps können beendet und neu gestartet werden, ohne sich erneut anmelden zu müssen. Durch die verifizierte Sitzung wird der Austausch der notwendigen Schlüssel zur Entschlüsselung von Nachrichten ermöglicht. <!--Alternativ kann eine verifizierte Matrixsitzung in einem privaten Browserfenster erstellt werden, indem man sich dort bei Matrix anmeldet und diese Sitzung aus einer bestehenden verifiziert. Dieses Fenster kann nach ungefähr fünf Minuten geschlossen werden. Die Schlüssel werden durch die Verifikation in die anderen Matrixclients übernommen. Das erzeugt eine Geistersitzung welche dann immer offen ist. Dann können alle anderen Clients abgemeldet werden. Ansonsten können Nachrichten welche in dem Zeitraum ohne offene Matrixsitzung empfangen werden später nicht mehr gelesen werden. Dies soll in Zukunft mittels der Funktion dehydrated devices gelöst werden.-->

#### Ich habe Schwierigkeiten beim Verifizieren einer neuen Sitzung {#verify-client}
1. Stellen Sie sicher, dass sie Ihren Sicherheitsschlüssel zur Verfügung haben. Andernfalls verlieren Sie durch die folgenden Schritte den Zugriff auf Ihre alten Nachrichten.
2. Logge Sie sich in den `Einstellungen` -> `Sitzungen` aus allen Clients aus.
3. Loggen Sie sich neu ein und verifizieren Sie die neue Sitzung durch Ihren Sicherheitsschlüssel.

#### Warum muss ich meinen Sicherheitsschlüssel speichern? {#store-securitykey}
* Mit Hilfe des _Sicherheitsschlüssels_ werden die persönlichen Schlüssel zur Kommunikation mit den Gesprächsteilnehmern verschlüsselt. Es handelt sich also quasi um eine Art "Universalschlüssel", der es ermöglicht die persönlichen Schlüssel in der [Schlüsselsicherung]({{< relref "first-steps/#einrichtung-der-schlüsselsicherung" >}}) zu speichern.
* Durch Eingabe des Sicherheitsschlüssels kann die Schlüsselsicherung abgerufen werden und eine neue Matrix-Sitzung verifiziert werden.
* Der Sicherheitsschlüssel besteht aus 12 Blöcken zu je vier Zeichen und startet mit einem großen E.
* Bei [Einrichtung der Schlüsselsicherung]({{< relref "first-steps/#einrichtung-der-schlüsselsicherung" >}}) empfiehlt es sich den Sicherheitsschlüssel in einem Passwortmanager, als Datei (in einem Sicheren Ordner! Nicht unter "Downloads") oder eventuell ausgedruckt zu speichern.
* Ohne den Sicherheitsschlüssel können keine neuen Sitzungen mehr verifiziert und keine Nachrichten mehr entschlüsselt werden, wenn man sich (eventuell unbeabsichtigt) von allen aktiven Matrix-Sitzungen abmeldet!

#### Was ist der Unterschied zwischen einem Sicherheitsschlüssel und einer Sicherheitsphrase? {#securitykey-vs-securityphrase}

* Da es schwierig ist sich den _Sicherheitsschlüssel_ zu merken, kann man sich eine (gut merkbare) _Sicherheitsphrase_ ausdenken (zum Beispiel einen [Passsatz](https://inv.13ad.de/watch?v=jtFc6B5lmIM)).
* Mit der _Sicherheitsphrase_ verschlüsselt der Matrixclient den _Sicherheitsschlüssel_.
* Durch das Anlegen einer (gut merkbaren) _Sicherheitsphrase_ wird das verifizieren einer neuen Matrix-Sitzung im Alltag (zum Beispiel unterwegs, wenn man nur fremde Rechner zur Verfügung hat) erleichtert.

#### Ich habe keinen Wiederherstellungsschlüssel
Bitte überprüfen Sie, ob die [Schlüsselsicherung](/settings/#schlüsselsicherung) eingerichtet wurde und richten diese ggf. neu ein.

#### Wie ändere ich die Sicherheitsphrase für meine Schlüsselsicherung? {#change-securityphrase}
Dazu rufen Sie im Element-Client die `Einstellungen` auf. Unter `Verschlüsselung` können Sie dann den `Wiederherstellungsschlüssel` ändern.

#### Wie kann ich die Schlüsselsicherung zurücksetzen, wenn ich meine Sicherheitsphrase UND meinen Sicherheitsschlüssel verloren habe? {#reset-securityphrase}
Bitte folgen Sie diesen Schritten:
1. In einer Matrix-Sitzung (=Client/Geräte/Browser), in der die früheren verschlüsselten Gespräche noch gelesen werden können, die Raumschlüssel exportieren. Dazu unter `Einstellungen`-> `Verschlüsselung` auf den Knopf "Schlüssel exportieren" klicken. Sollte es keinen Zugang zu irgendeiner Matrix-Sitzung mehr geben, in der frühere verschlüsselte Nachrichten lesbar sind, diesen Schritt überspringen.
2. In der gleichen Matrix-Sitzung, in der in Schritt 1 die Raumschlüssel manuell exportiert wurden, unter `Einstellungen`-> `Sitzungen` alle anderen Sitzungen über die Checkbox am Zeilenanfang markieren und unterhalb der Liste auf den roten Knopf "abmelden" klicken.
3. Gegebenenfalls ausloggen und wieder einloggen, dabei Nachfragen ignorieren.
4. Unter `Einstellungen`-> `Verschlüsselung` schauen ob dort ein grüner Knopf `Einrichten` und keine roten Knöpfe da sind. Wenn noch rote Knöpfe da sind, erst den Knopf `Kryptografische Identität zurücksetzen` auswählen. Möglicherweise ist ein Abmelden und erneutes Anmelden notwendig.
5. Jetzt die zuvor exportieren Schlüsselsicherungen manuell importieren. Dazu unter `Einstellungen`-> `Verschlüsselung` auf `Schlüssel importieren` klicken.
6. Neue [Schlüsselsicherung]({{< relref "settings/#schlüsselsicherung" >}}) einrichten und den neuen Sicherheitsschlüssel an verschiedenen Orten sicher aufbewahren.

***
### Allgemeines

#### Wie teilt man Leuten mit dem Element-Client eine Raumadresse mit? {#share-room}
Mit dem matrix.to-Link, den man unter dem i für die Raumeigenschaften und einem weiteren Klick auf „Teile Raum“ erhält.

#### Wie kann man in einer Gruppe, in der sich der einzige Admin entfernt hat, wieder einen Admin neu definieren? {#no-admin}
Grundsätzlich ist der Raum dann "verloren" und hat keinen Admin mehr. InnoCampus kann aber auf Anfrage entweder den Raum löschen oder einen anderen Nutzenden zum Admin ernennen. Um dieses Angebot wahrzunehmen, bitte eine Anfrage an den Servicedesk mit der Raum-Adresse `#<roomname>:tu-dresden.de` und dem zukünftigen Admin `@<username>:tu-dresden.de` senden. Wir kontrollieren dann, dass es tatsächlich keinen anderen Admin mehr gibt. Es bleibt aber die Frage offen, warum die genannte Person dann zum neuen Admin werden sollte. Im Zweifel ist das Löschen und neu Anlegen des Raumes also die bessere Lösung.

#### Kann ich LaTeX schreiben? {#latex}
Ja! Zur Zeit ist es nur ein experimentelles Feature, aber in wenigen Wochen wird es für alle verfügbar sein. Siehe https://github.com/vector-im/element-web/issues/1945
Das Experimentelle Feature kann in den Einstellungen unter **Labor** aktiviert werden.

#### Gibt es etwas ähnliches wie Threads (vgl. Mattermost/Slack) in Matrix? {#threads}
Threads sind in Kürze in Matrix verfügbar und aktuell, zumindest am Element Desktop, als Laborfunktion verfügbar: https://github.com/vector-im/roadmap/projects/1

#### Warum gibt es keinen Raum "TU Dresden"? Wer dürfte ihn erstellen? {#no-tud-room}
Alle Personen, die einen Raum erstellt haben, sind administrierende Personen und tragen die Verantwortung für den Raum. Matrix ist bisher nicht für den Austausch von tausenden Mitgliedern an der Universität gedacht. Sollte eines Tages ein zentraler Raum von Bedarf sein, würde die Einrichtung und Pflege von InnoCampus übernommen werden.

<!--
#### Wie kann ich als administrierende Person viele Nachrichten auf einmal löschen? {#delete-multiple-messages}
?-->

#### Ich kann mich über die Element IOS-App nicht anmelden {#apple-anmeldung}
Anders als in der Installationsanleitung dargestellt, kann man in der iOS-App nicht auf `https://` vor der Serveradresse `tu-dresden.de` verzichten, wie es bei der Android-App der Fall ist.

#### Was muss ich tun, wenn auf einem MacOS Video oder Audio in einer Videokonferenz nicht funktioniert? {#apple-no-video}
Häufig hat Element nicht die Rechte, auf die Webcam und das Mikrofon zu zugreifen. Diese können in den Systemeinstellungen unter Sicherheit und Privatsphäre vergeben werden.

#### Wie viele Personen können gleichzeitig in einen Raum eingeladen werden? Kann ich Personen über ihre E-Mail-Adressen einladen? {#how-many-invites-can-i-do}
Die Masseneinladung per E-Mail wird derzeit in Element nicht unterstützt. Wenn Sie eine Masseneinladung durchführen möchten, senden Sie bitte eine Anfrage an den Servicedesk, damit wir Ihnen helfen können. Sie können selbst bis zu 25 Personen über ihren Account einladen.

#### Kann ich mit Element mehrere Matrix-Accounts verwalten (Multi-Account-Client)? {#multiple-accounts-element}
Ein Element-Fenster kann zur Zeit nur einen Matrix-Account verwalten. Es ist aber möglich, mehrere Element-Fenster mit unterschiedlichen Matrix-Konten zu starten, auch im Autostart des Rechners. Dazu ist der Programmaufruf so abzuändern, dass ein spezifisches Profil geöffnet wird:
```
element-desktop --profile PROFILNAME
```
So lassen sich mehrere Starter im Autostart platzieren, die dann verschiedene Profilnamen haben, z.B. --profile TUB und --profile Privat. Beide geöffneten Fenster haben leider die gleichen Icons im Indicator-Applet. Hierfür gibt es aber sicher auch bald eine Lösung.

Darüber hinaus gibt es andere Matrix-Clients, die mehrere Matrix-Konten verwalten können. Zum Beispiel [weechat](https://matrix.org/docs/projects/client/weechat-matrix), [Spectral](https://matrix.org/docs/projects/client/spectral), [Quaternion](https://matrix.org/docs/projects/client/quaternion) oder [Mirage](https://matrix.org/docs/projects/client/mirage).

#### Überall steht nur „missing translation: en“ {#missing-translations}
Dieses Phänomen steht häufig im Zusammenhang mit noch nicht fertiggestellten Aktualisierungen des Matrix-Clients. Laden Sie den Zwischenspeicher neu. Dazu gehen Sie in den Element-Einstellungen in die Kategorie „Hilfe und Info“. Scrollen Sie ganz nach unten und wählen „Zwischenspeicher löschen und neu laden“.

#### Ist unser Server auf eurer Föderations-Blacklist? {#blacklist}
Aktuell befindet sich kein Server auf unserer Föderations-Blacklist. Dies kann nicht der Grund für etwaige Föderations-Probleme sein.

#### Ich sehe in einem Raum von einer bestimmten Person keine Nachrichten {#blocked-user}
Ein häufig vorkommender Grund hierfür ist, dass Sie sich verklickt haben und die Person, von der Sie keine Nachrichten mehr sehen, obwohl Ihnen berichtet wird, dass dort etwas stehen müsste, von Ihnen blockiert wurde. Öffnen Sie hierzu Ihre Sicherheitseinstellungen und scrollen weit nach unten. Prüfen Sie, ob in der Kategorie „Blockierte Benutzer“ Einträge stehen, die dort nicht hingehören. Entfernen Sie diese gegebenenfalls.

#### Warum sieht man im Element Desktop-Client keine Statuszeile am unteren Ende des Bildschirms wenn man die Maus über Hyperlinks bewegt? {#no-statusline}
Tatsächlich ist die Statusleiste eine beliebte Prüfung der Seriösität von Hyperlinks, die man versucht ist anzuklicken. Im Element Desktop Client und mobilen Clients geht das leider nicht. Hier kann man nur mit der rechten Maustaste auf den Link klicken und so die präsentierte Zielseite auf Seriösität prüfen.