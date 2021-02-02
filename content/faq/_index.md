---
menutitle: "Häufige Fragen (FAQ)"
title: "Häufig gestellte Fragen"
date: 2020-08-02T21:26:25+02:00
draft: false
weight: 200
---
Dies ist eine Zusammenstellung häufiger Fragen und deren Antworten. Teilweise sind die Antworten noch nicht formuliert. In diesen Fällen bitte im Raum ```#matrix-support:tu-dresden.de``` nachfragen.

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

***
#### Was ist der Unterschied zwischen Sicherheitsphrase und Sicherheitsschlüssel? {#securityphrase-vs-securitykey}
Das Passwort, das auf die Schlüsselsicherung zugreifen kann, wird Sicherheitsschlüssel genannt und ist sehr lang, beginnt mit einem großen E und sollte nach dem Einrichten gespeichert oder ausgedruckt werden. Da dieses Passwort im Alltag schlecht gemerkt werden kann (bspw. unterwegs, wenn man mal eben in Matrix vorbeischauen möchte, aber nur fremde Rechner zur Verfügung hat) kann man sich eine (gut merkbare) Sicherheitsphrase ausdenken, aus der der Sicherheitsschlüssel (im Browser/Client) errechnet werden kann, bevor versucht wird, die Schlüsselsicherung „zu öffnen“.
***
#### Warum sieht man im Element Desktop-Client keine Statuszeile am unteren Ende des Bildschirms wenn man über Hyperlinks hovert (= Maus drüber bewegt und verweilt)? Wie kann man diesen dann vertrauen? {#no-statusline}
Tatsächlich ist die Statusleiste eine beliebte Prüfung der Seriösität von Hyperlinks, die man versucht ist anzuklicken. Im Element Desktop Client geht das ähnlich der mobilen Clients nicht. Hier kann man nur mit der rechten Maustaste auf den Link klicken und so die präsentierte Zielseite auf Seriösität prüfen.
***
#### Wie teilt man Leuten mit Element Desktop-Client eine Raumadresse mit? {#desktop-share-room}
Mit dem matrix.to-Link, den man unter dem i für die Raumeigenschaften und einem weiteren Klick auf „Teile Raum“ erkennt.
***
#### Wie teilt man Leuten mit Element Web-Client eine Raumadresse mit? {#web-share-room}
Mit dem matrix.to-Link, den man unter dem i für die Raumeigenschaften und einem weiteren Klick auf „Teile Raum“ erkennt und einem Austausch vom vorderen matrix.to mit matrix.tu-dresden.de
***
#### Kann ich LaTeX schreiben? {#latex}
Ja! Zur Zeit ist es nur ein experimentelles Feature, aber in wenigen Wochen wird es für alle verfügbar sein. Siehe https://github.com/vector-im/element-web/issues/1945

***
#### Gibt es sowas wie Threads (vgl. Mattermost/Slack) in Matrix? {#threads}
Threads sind bisher noch nicht in Matrix verfügbar. Das Thema ist aber bei den Entwickler:innen bekannt und wurde in die Entwicklungsperspektive mit aufgenommen und sollte in Zukunft integriert werden. Verfolge dazu: https://github.com/vector-im/roadmap/projects/1

***
#### Ich habe keinen Wiederherstellungsschlüssel
Dafür bitte prüfen, ob diese überhaupt eingerichtet wurde. Siehe [Schlüsselsicherung](/settings/#schlüsselsicherung)

***
#### Wie ändere ich die Sicherheitsphrase für meine Schlüsselsicherung? {#change-securityphrase}
?
***
#### Wie kann ich die Schlüsselsicherung zurücksetzen, wenn ich meine Sicherheitsphrase UND meinen (abgespeicherten und ausgedruckten) Sicherheitsschlüssel verloren habe? {#reset-securityphrase}

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
#### Kann ich die Beitrittsrechte aller Räume meiner Community so anpassen, dass nur Mitglieder der Community Zutritt haben? {#roompermissions-in-communities}
Nein, dies ist nicht möglich. Räume können in mehreren Communities sein. Der Zutritt zu Räumen wird daher raumweise eingestellt. 
