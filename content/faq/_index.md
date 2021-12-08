---
menutitle: "Häufige Fragen (FAQ)"
title: "Häufig gestellte Fragen"
date: 2020-08-02T21:26:25+02:00
draft: false
weight: 200
---
Dies ist eine Zusammenstellung häufiger Fragen und deren Antworten. Teilweise sind die Antworten noch nicht formuliert. In diesen Fällen bitte im Raum ```#matrix-support:tu-dresden.de``` nachfragen.

* [Nachrichten nicht lesbar](#unable-to-decrypt)
* [Was ist der Unterschied zwischen Sicherheitsphrase und Sicherheitsschlüssel?](#securityphrase-vs-securitykey)
* [Warum sieht man im Element Desktop-Client keine Statuszeile am unteren Ende des Bildschirms wenn man über Hyperlinks hovert (= Maus drüber bewegt und verweilt)? Wie kann man diesen dann vertrauen?](#no-statusline)
* [Wie teilt man Leuten mit Element Desktop-Client eine Raumadresse mit?](#desktop-share-room)
* [Wie teilt man Leuten mit Element Web-Client eine Raumadresse mit?](#web-share-room)
* [Kann ich LaTeX schreiben?](#latex)
* [Gibt es sowas wie Threads (vgl. Mattermost/Slack) in Matrix?](#threads)
* [Wie ändere ich die Sicherheitsphrase für meine Schlüsselsicherung?](#change-securityphrase)
* [Wie kann ich die Schlüsselsicherung zurücksetzen, wenn ich meine Sicherheitsphrase UND meinen (abgespeicherten und ausgedruckten) Sicherheitsschlüssel verloren habe?](#reset-securityphrase)
* [Warum gibt es keinen Raum „TU Dresden“? Wer dürfte ihn erstellen?](#no-tud-room)
* [Wie kann ich als administrierende Person viele Nachrichten auf einmal löschen?](#delete-multiple-messages)
* [Manchmal sehe ich einen fett markierten Raum und klicke ihn an, habe aber doch nicht die Zeit, den Inhalt und etwaige Konsequenzen für mich sofort zu bearbeiten. Wie kann ich den Raum wieder als „ungelesen“ markieren?](#mark-room-as-unread)
* [Was muss ich tun, wenn auf einem MacOS Video oder Audio in einer Videokonferenz nicht funktioniert.](#apple-no-video)
* [Wie viele Personen können gleichzeitig in einen Raum eingeladen werden? Kann ich Personen über ihre E-Mail-Adressen einladen?](#how-many-invites-can-i-do)
* [Kann ich die Beitrittsrechte aller Räume meiner Community so anpassen, dass nur Mitglieder der Community Zutritt haben?](#roompermissions-in-communities)
* [Kann ich mit Element mehrere Matrix-Accounts verwalten (Multi-Account-Client)?](#multiple-accounts-element)
* [Ich kann keine Profil-/Raumbilder oder gesendete Bilder mehr sehen.](#relogin)
* [Überall steht nur „missing translation: en“|](#missing-translations)
* [Ist unser Server auf eurer Föderations-Blacklist?](#blacklist)
* [Ich sehe in einem Raum von einer bestimmten Person keine Nachrichten](#blocked-user)

***
#### Nachrichten nicht lesbar{#unable-to-decrypt}
  * Es muss zur zeit mindestens immer eine verifizierte Sitzung offen sein, am einfachsten geht dies, wenn der Desktop Client oder Element auf dem tragbarem Handrechner eingerichtet ist. Diese Programme können beendet und neu gestartet werden, ohne sich erneut anmelden zu müssen. Anderweitig kann eine verifizierte Matrixsitzung in einem privaten Browserfenster erstellt werden, indem man sich dort bei Matrix anmeldet und diese Sitzung aus einer bestehenden verifziert. Dieses Fenster kann nach ca. fünf Minuten geschlossen werden. Die Schlüssel werden durch die Verifikation in die anderen Matrixclients übernommen. Das erzeugt eine Geistersitzung welche dann immer offen ist. Dann können alle anderen Clients abgemeldet werden. Ansonsten können Nachrichten welche in dem Zeitraum ohne offene Matrixsitzung empfangen werden später nicht mehr gelesen werden. Dies soll in Zukunft mittels der Funktion dehydrated devices gelöst werden.
  * Wurde die Schlüsselsicherung ordnungsgemäß eingerichtet?
  * Nachrichten bleiben nicht lesbar, wenn Matrixsitzungen erstellt werden und dann das Fenster des Browsers einfach geschlossen wird, ohne sich abzumelden. Lösung: nur für neue Nachrichten möglich: diese Dokumentation durchlesen.

***
#### Was ist der Unterschied zwischen Sicherheitsphrase und Sicherheitsschlüssel? {#securityphrase-vs-securitykey}
Das Kennwort, welches für die Schlüsselsicherung benötigt wird heißt Sicherheitsprase. Damit verschlüssel der Matrixclient den Sicherheitsschlüssel/Wiederherstellungsschlüssel. Der Sicherheitsschlüssel wird beim erstellen als security-key.txt angeboten und sollte bei Windows nicht unter Downloads gespeichert werden, da dieser von Windows gegebenenfalls automatisch bereinigt wird. Der Sicherheitsschlüssel besteht aus 12 Blöcken zu je vier Zeichen und startet mit einem großen E. Es empfiehlt sich nach dem Einrichten des Sicherheitsschlüssels diesen in einem Passwortmanager, als Datei und evlt. ausgedruckt zu speichern. Da der Sicherheitsschlüssel im Alltag schlecht gemerkt werden kann (bspw. unterwegs, wenn man mal eben in Matrix vorbeischauen möchte, aber nur fremde Rechner zur Verfügung hat) kann man sich eine (gut merkbare) Sicherheitsphrase ausdenken (z.B. ein [Passsatz](https://inv.13ad.de/watch?v=jtFc6B5lmIM)), damit kann dann die Sitzung verifiziert werden und wird damit mit der Schlüsselsicherung verbunden.
***
#### Warum sieht man im Element Desktop-Client keine Statuszeile am unteren Ende des Bildschirms wenn man über Hyperlinks hovert (= Maus drüber bewegt und verweilt)? Wie kann man diesen dann vertrauen? {#no-statusline}
Tatsächlich ist die Statusleiste eine beliebte Prüfung der Seriösität von Hyperlinks, die man versucht ist anzuklicken. Im Element Desktop Client geht das ähnlich der mobilen Clients nicht. Hier kann man nur mit der rechten Maustaste auf den Link klicken und so die präsentierte Zielseite auf Seriösität prüfen.
***
#### Wie teilt man Leuten mit Element Desktop-Client eine Raumadresse mit? {#desktop-share-room}
Mit dem matrix.to-Link, den man unter dem i für die Raumeigenschaften und einem weiteren Klick auf „Teile Raum“ erkennt.
***
#### Wie teilt man Leuten mit Element Web-Client eine Raumadresse mit? {#web-share-room}
Mit dem matrix.to-Link, den man unter dem i für die Raumeigenschaften und einem weiteren Klick auf „Teile Raum“ erkennt und einem Austausch vom vorderen matrix.to/#/ mit matrix.tu-dresden.de/#/room/
***
#### Kann ich LaTeX schreiben? {#latex}
Ja! Zur Zeit ist es nur ein experimentelles Feature, aber in wenigen Wochen wird es für alle verfügbar sein. Siehe https://github.com/vector-im/element-web/issues/1945

***
#### Gibt es sowas wie Threads (vgl. Mattermost/Slack) in Matrix? {#threads}
Threads sind in Kürze in Matrix verfügbar und aktuell, zumindest am Element Desktop, als Laborfunktion ausprobierbar: https://github.com/vector-im/roadmap/projects/1

***
#### Ich habe keinen Wiederherstellungsschlüssel
Dafür bitte prüfen, ob diese überhaupt eingerichtet wurde. Siehe [Schlüsselsicherung](/settings/#schlüsselsicherung)

***
#### Wie ändere ich die Sicherheitsphrase für meine Schlüsselsicherung? {#change-securityphrase}
  * bei allen Matrix-Sitzungen bis auf eine, auf die noch Zugriff besteht, die Raumschlüssel exportieren `Einstellungen`-> `Sicherheit & Datenschutz` -> `Verschlüsselung` hier am besten mit dem Matrixanmeldekennwort versehen. Abschließend abmelden, dafür links oben auf den Benutzernamen und abmelden, bei der Frage möglicherweise auftretenden Fage ob die verschüsselten Nachrichten gewünscht werden den Knopf `Ich möchte meine verschlüsselten Nachrichten nicht` betätigen, da diese Schlüssel eben schon exportiert wurden.
  * Unter `Einstellungen`-> `Sicherheit & Datenschutz` -> `Sicheres Backup` erst den Knopf `Sicherung löschen`, dann den Knopf `Zurücksetzen`, möglicherweise ist ein löschen des Zwischenspeichers unter `Einstellungen`-> `Hilfe & Über` nötig, möglicherweise auch ein abmelden und erneutes anmelden mit anschließendem erneuten Versuch. Wenn das alles nicht geht, im nächsten Punkt fortfahren. Die Aktion war erfolgreich, wenn nur noch der grüne Einrichten Knopf angezeigt wird.
  * Für alle vorher exportieren Schlüsselsicherungen den manuellen importweg ausführen.
  * Neue Schlüsselsicherung einrichten. Siehe [Schlüsselsicherung](/settings/#schlüsselsicherung)

***
#### Wie kann ich die Schlüsselsicherung zurücksetzen, wenn ich meine Sicherheitsphrase UND meinen (abgespeicherten und ausgedruckten) Sicherheitsschlüssel verloren habe? {#reset-securityphrase}
Bitte folgendes ausführen:
  * bei allen Matrix-Sitzungen bis auf eine, auf die noch Zugriff besteht, die Raumschlüssel exportieren `Einstellungen`-> `Sicherheit & Datenschutz` -> `Verschlüsselung` hier am besten mit dem Matrixanmeldekennwort versehen. Abschließend abmelden, dafür links oben auf den Benutzernamen und abmelden, bei der Frage möglicherweise auftretenden Fage ob die verschüsselten Nachrichten gewünscht werden den Knopf `Ich möchte meine verschlüsselten Nachrichten nicht` betätigen, da diese Schlüssel eben schon exportiert wurden.
  * alle Sitzungen auf die kein Zugriff mehr besteht [löschen]({{< relref "settings/#sicherheit--datenschutz" >}}) die oberste in Fettschrift ist die aktuelle Sitzung, diese nicht mit anhaken
  * die letzte Sitzung abmelden
  * Eine Nachricht an den Servicedesk schreiben, mit der Bitte in der Datenbank die Sicherheitsschlüssel zu löschen
  * auf die Antwort warten
  * bei Matrix anmelden und bei den Fenstern und Meldungen die Verifikation überspringen
  * bei Matrix abmelden
  * bei Matrix erneut anmelden und bei den Fenstern und Meldungen die Verifikation überspringen
  * Unter `Einstellungen`-> `Sicherheit & Datenschutz` -> `Sicheres Backup` schauen ob dort ein grüner Knopf `Einrichten` und keine roten Knöpfe da sind. Wenn noch rote Knöpfe da sind, erst den Knopf `Sicherung löschen`, dann den Knopf `Zurücksetzen` möglicherweise ist ein löschen des Zwischenspeichers unter `Einstellungen`-> `Hilfe & Über` nötig, möglicherweise auch ein abmelden und erneutes anmelden. Ebenso kann es sein, das unter `Einstellungen`-> `Sicherheit & Datenschutz` -> `Cross-Signing` auf den roten Knopf `Zurücksetzen` gedrückt werden muss. Die Aktion war erfolgreich, wenn für `Sicheres Backup` und `Cross-Signing` nur noch der grüne Einrichten Knopf angezeigt wird.
  * wenn das alles nicht geht auf das Ticket antworten mit der Bitte um eine Jitsibesprechung
  * Für alle vorher exportieren Schlüsselsicherungen den manuellen importweg ausführen.
  * Neue Schlüsselsicherung einrichten. Siehe [Schlüsselsicherung]({{< relref "settings/#schlüsselsicherung" >}})

***
#### Warum gibt es keinen Raum „TU Dresden“? Wer dürfte ihn erstellen? {#no-tud-room}
Alle raumerstellenden Personen sind administrierende Personen und tragen die Verantwortung für den Raum. Matrix ist bisher nicht für den Austausch von tausenden Mitgliedern an der Universität gedacht. Sollte eines Tages ein zentraler Raum von Bedarf sein, würde die Einrichtung und Pflege sicher beim Rektorat und dem Dezernat „Strategie & Kommunikation“ liegen.
***
#### Wie kann ich als administrierende Person viele Nachrichten auf einmal löschen? {#delete-multiple-messages}
?
***
#### Manchmal sehe ich einen fett markierten Raum und klicke ihn an, habe aber doch nicht die Zeit, den Inhalt und etwaige Konsequenzen für mich sofort zu bearbeiten. Wie kann ich den Raum wieder als „ungelesen“ markieren? {#mark-room-as-unread}
Das geht in Element leider nicht. Als Workaround kann man den Raum als Favorit markieren und sich selbst merken, dass eigene Favoriten nochmal in den Blick genommen werden sollten.

***
#### Was muss ich tun, wenn auf einem MacOS Video oder Audio in einer Videokonferenz nicht funktioniert. {#apple-no-video}
Häufig hat Element nicht die Rechte, auf die Webcam und das Mikrofon zu zugreifen. Diese können in den Systemeinstellungen unter Sicherheit und Privatsphäre vergeben werden.

***
#### Wie viele Personen können gleichzeitig in einen Raum eingeladen werden? Kann ich Personen über ihre E-Mail-Adressen einladen? {#how-many-invites-can-i-do}
Die Masseneinladung per E-Mail wird derzeit in Element nicht unterstützt. Wenn Sie eine Masseneinladung durchführen möchten, senden Sie bitte eine Anfrage über den Servicedesk, damit wir Ihnen helfen können. Sie können selbst 100 Personen über ihren ZIH-Benutzernamen einladen.

***
#### Kann ich mit Element mehrere Matrix-Accounts verwalten (Multi-Account-Client)? {#multiple-accounts-element}
Ein Element-Fenster kann zur Zeit nur einen Matrix-Account verwalten. Es ist aber möglich, mehrere Element-Fenster mit unterschiedlichen Matrix-Konten zu starten, auch im Autostart des Rechners. Dazu ist der Programmaufruf so abzuändern, dass ein spezifisches Profil geöffnet wird:
```
element-desktop --profile PROFILNAME
```
So lassen sich mehrere Starter im Autostart platzieren, die dann verschiedene Profilnamen haben, z.B. --profile TUD und --profile Privat. Beide geöffneten Fenster haben leider gleichaussehende Icons im Indicator-Applet. Hierfür gibt es aber sicher auch bald eine Lösung...

Darüber hinaus gibt es andere Matrix-Clients, die mehrere Matrix-Konten verwalten können, u.a. [weechat](https://matrix.org/docs/projects/client/weechat-matrix), [Spectral](https://matrix.org/docs/projects/client/spectral), [Quaternion](https://matrix.org/docs/projects/client/quaternion) oder [Mirage](https://matrix.org/docs/projects/client/mirage).

***
#### Ich kann keine Profil-/Raumbilder oder gesendete Bilder mehr sehen. {#relogin}
Aufgrund einer Aktualisierung am Matrix Server (28.03.2021) finden Clients, die seitdem angemeldet sind, keine Mediendateien mehr. Um dieses Problem zu lösen, ist ein Ab- und erneutes Anmelden notwendig. **Damit Sie keine Ihrer Nachrichten verlieren sollten Sie folgendes Vorgehen beachten:** Sind mehrere Clients betroffen, so sollte die Prozedur nacheinander pro Client durchgeführt werden und nicht parallel.

<ul type="1">
  <li>Stellen Sie sicher, dass Sie mindestens einen Punkt erfüllt haben:</li>
  <ol type="a">
    <li>... eine zusätzliche verifizierte Sitzung (z.B. mit dem Smartphone) ist aktiv und benutzbar</li>
    <li>... die <a href="{{< relref "settings/#schlüsselsicherung" >}}">Schlüsselsicherung</a> ist eingerichtet und die Sicherheitsphrase oder der Sicherheitsschlüssel ist vorhanden</li>
    <li>... die Raumschlüssel sind exportiert wurden</li>
  </ol>
  <li>Melden Sie sich im Client ab und erneut an und verwenden Sie als <strong>Heimserver:</strong> "<strong>tu-dresden.de</strong>"</li>
  <li>Stellen Sie Ihre Nachrichten wieder her:</li>
  <ol type="a">
    <li>... Verifizieren Sie die neue Sitzung in einer zusätzlichen aktiven Sitzung (z.B. mit dem Smartphone), um den Schlüsselaustausch zwischen diesen Sitzungen zu starten</li>
    <li>... Verbinden Sie sich mit der Schlüsselsicherung, um Ihre Nachrichtenschlüssel zurück zu erhalten</li>
    <li>... Importieren Sie die Raumschlüssel und richten Sie die <a href="{{< relref "settings/#schlüsselsicherung" >}}">Schlüsselsicherung</a> ein</li>
  </ol>
</ul>

* **Anmerkungen:**
  * Das Verlieren der Raumschlüssel führt zum Verlust Ihrer Nachrichten, da diese nur für Sie und ihre Kommunikationsteilnehmer:innen lesbar sind. Da kann kein Admin helfen.
  * Aufgrund der neuen Sitzung wird anschließend bei allen Ihrer früheren Nachrichten ein rotes Warnschild anzeigt. Das ist kein Fehler, sondern nur eine etwas zu dramatisch eingestellte Information (Diskussionen diesbzgl. gibt es hier: [externer Link](https://github.com/vector-im/element-web/issues/13701))
  * Sollten Sie Matrix nur auf einem Gerät nutzen und derzeit keinen Zugriff auf Ihre schon eingerichtete Schlüsselsicherung haben (also die Sicherheitsphrase oder den Sicherheitsschlüssel nicht finden, dann müssen Sie Option c) folgen um keinen Verlust Ihrer verschlüsselten Nachrichten zu erfahren)


#### Überall steht nur „missing translation: en“ {#missing-translations}

Dieses Phänomen steht häufig im Zusammenhang mit noch nicht fertiggestellten Aktualisierungen des Matrix-Clients. Laden Sie den Zwischenspeicher neu: Gehen Sie in den Element-Einstellungen in die Kategorie „Hilfe und Über“ und scrollen Sie ganz nach unten: „Zwischenspeicher löschen und neu laden“ sollte das Anzeigeproblem beheben.

#### Ist unser Server auf eurer Föderations-Blacklist? {#blacklist}

Aktuell befindet sich kein Server auf unserer Föderations-Blacklist. Dies kann nicht der Grund für etwaige Förderations-Probleme sein.


#### Ich sehe in einem Raum von einer bestimmten Person keine Nachrichten {#blocked-user}

Ein häufig vorkommender Grund hierfür ist, dass Sie sich verklickt haben und die Person, von der Sie keine Nachrichten mehr sehen, obwohl Ihnen berichtet wird, dass dort etwas stehen müsste, von Ihnen blockiert wurde. Öffnen Sie hierzu Ihre Sicherheitseinstellungen und scrollen weit nach unten. Prüfen Sie, ob in der Kategorie „Blockierte Benutzer“ Einträge stehen, die dort nicht hingehören. Entfernen Sie diese ggf.
