---
title: "Erste Schritte"
date: 2020-08-02T21:26:25+02:00
chapter: true
draft: false
weight: 2
---

# Erste Schritte - Wie kann Matrix genutzt werden?

## Matrix-Login mit ZIH-Account

Mitgliedern und Angehörigen der TU Dresden (selbstverständlich auch Studierenden) wird unter Einhaltung der einschlägigen gesetzlichen und rechtlichen Bestimmungen zum Datenschutz und zur IT-Sicherheit ermöglicht, mittels ihres **ZIH-Logins** mit Angehörigen dieser und anderer Hochschulen und Universitäten sowie weiteren Matrix-Nutzenden (bspw. akademischen Partner:innen) per Chat sowie Audio-/Video-Telefonie zu kommunizieren.

{{% notice tip %}}
Wir empfehlen die Nutzung des Element Desktopclients, weil so zahlreiche Probleme, die bei dem Nutzen der Verschlüsselung entstehen können, vermieden werden können.
{{% /notice %}}

Downloads für: {{% button href="https://packages.riot.im/desktop/install/win32/x64/Element%20Setup.exe" icon="fas fa-download" %}}Windows{{% /button %}} {{% button href="https://packages.riot.im/desktop/install/macos/Element.dmg" icon="fas fa-download" %}}macOS{{% /button %}} {{% button href="/clients/install_linux" icon="fas fa-download" %}}Linux{{% /button %}}

Nach einer Desktop-Installation ist darauf zu achten, den bestehenden Account mit dem ZIH-Login zu nutzen, und keinen neuen Account auf einem anderen Server zu erstellen. Hier am Beispiel von Element:

![Markierter Anmeldebutton im Element Matrixclient](/images/01_Login_de.png)

Dies wird durch Klick auf **Ändern** realisiert. Dann landet man nicht versehentlich auf einem falschen Server...

![Anmeldeseite mit Fokus auf dem Homeserver ändern Button](/images/02_Change-Homeserver_de.png)

Nun kann man manuell die Angabe des Heimservers durchführen: tu-dresden.de

![Eingabefeld zum Ändern des Homeservers mit der Eingabe matrix.tu-dresden.de](/images/03_Set-Homeserver_de.png)

Anschließend ist der einmalige Login mit ZIH-Login und ZIH-Passwort durchzuführen:
Dropdown-Menü „Anmelden mit:“ sollte auf „Benutzername“ belassen werden. Dann sind folgende Eingaben zu tätigen:

**Benutzername: ZIH-Login**  (nur der ZIH-Login, keine E-Mail-Adresse!)

**Passwort: ZIH-Passwort**

Ein alternativer Login, bspw. über die E-Mail-Adresse ist **NICHT** beim ersten, initialen, Anmelden möglich, erst ab dem zweiten Einloggen.

Es folgt nach dem Erstlogin auch keine E-Mail / Bestätigungsmail.

Analog zu E-Mail-Adressen ergeben sich damit Matrix-Adressen folgender Struktur:

@ZIH-Login:tu-dresden.de

![Loginfenster mit Aufforderung ZIH Login und Passwort einzugeben](/images/04_Username_de.png)

## Bequemes Nutzen der Ende-zu-Ende-Verschlüsselung (E2EE)

Matrix verschlüsselt nicht nur die Transporte von und zu dem Heimserver (im Rechenzentrum der TU Dresden) sondern erlaubt auch die Nutzung von Ende-zu-Ende-Verschlüsselung (E2EE). Hierzu müssen kryptografische Schlüssel zwischen allen Geräten ausgetauscht werden, die sich Ende-zu-Ende-verschlüsselt schreiben möchten. Obwohl diese technische Notwendigkeit kompliziert klingt und im Hintergrund auch ist, ist sie inzwischen für die Anwendenden sehr bequem geworden. Die vielen kryptografischen Schlüssel werden vom Client erstellt auf dem jeweiligen Gerät gespeichert. Sollte dies bspw. ein Tab in einem Browser sein, besteht die Gefahr, dass dieser Tab einmal unbeabsichtigt geschlossen wird. Dann sind alle verschlüsselten Inhalte nicht mehr lesbar. Damit dies nicht geschieht, wird eine Schlüsselsicherung auf dem Heimserver der TU Dresden angeboten, auf der (mit einer Sicherheitsphrase (bzw. daraus errechenbaren Sicherheitsschlüssel) geschützt) alle kryptografischen Schlüssel verschlüsselt abgelegt sind.

{{% notice info %}}
Es wird dringend empfohlen, die Schlüsselsicherung zu nutzen (mit einer sicheren Sicherheitsphrase, welche NICHT Ihr ZIH-Passwort ist)!
{{% /notice %}}

![Aufforderung den Sicherheitsschlüssel zu generieren oder eine Sicherheitsphrase einzugeben](/images/11_Setup-Key_de.png)
![Aufforderung eine Passwort für die Schlüsselsicherung einzugeben](/images/12_Enter-Key_de.png)
Alternativ können Sie sich statt der Sicherheitsphrase auch einen Sicherheitsschlüssel generieren lassen, welcher den selben Zweck wie die Sicherheitsphrase erfüllt. Weiterhin wird der Sicherheitsschlüssel immer zusätzlich zur Sicherheitsphrase erstellt und sollte als Notfallschlüssel sicher und wiederauffindbar verwahrt werden (z.B. Abspeichern als .txt-Datei UND Ausdrucken) 
![Anzeige des Sicherheitsschlüssel zum abschreiben oder wegspeichern](/images/13_Present-Key_de.png) 

[Weitere wichtige Einstellungen]({{< relref "settings/_index.md" >}}) können Ihr Matrix-Erlebnis verbessern!


## Aufforderungen zum Einrichten der Schlüsselsicherung

![Screenshot der Aufforderung eine Sicherheitsphrase einzugeben](/images/01_Restore-Session_de.png)

Sollte die Aufforderung zum Einrichten der Schlüsselsicherung übersprungen werden, sähe der nächste Bildschirm so aus:

![Bestätigung des Überspringens der Eingabe einer Sicherheitsphrase](/images/03_Cancel-Restore_de.png)

Die Schlüsselsicherung wird dringend empfohlen, um sorgenfrei Ende-zu-Ende-Verschlüsselung nutzen zu können. Daher wird auch nach einem weiteren Überspringen in einem kleineren Tooltip zur Einrichtung der Verschlüsselung aufgefordert:

![Chatansicht mit der Anzeige eines Tooltips, Verschlüsselung einzurichten. Markierung des bestätigen Feldes](/images/04_Notification_de.png)

Sollten Sie dies auch hier auslassen wird Ihnen eine letzte Warnung bei einem bewussten Abmelden angezeigt. Wenn spätestens hierbei keine Schlüsselsicherung eingerichtet wird, kann später auf ggf. schon stattgefundene verschlüsselte Gespräche nicht mehr zugegriffen werden. Sollte der Tab geschlossen werden, entspricht dies ggf. ebenfalls einem Abmelden.

![Abfrage, ob Nachrichten verschlüsselt werden sollen](/images/05_Logout-Notify_de.png)

Vermeiden Sie diese Situation durch eine eingerichtete Schlüsselsicherung!

## Matrix-Login ohne ZIH-Account

Eine Registrierung von Accounts (wie vllt. von anderen Matrix-Servern bekannt) ist hier an der TU Dresden nicht möglich, da den Dienst ausschließlich Personen mit ZIH-Login nutzen können. Die TU Dresden ist kein Kommunikationsdiensteanbieter.

Für wissenschaftliche Kooperationen mit Kolleg:innen ohne ZIH-Account besteht die Möglichkeit zur [Beantragung eines ZIH-Gast-Accounts](https://tu-dresden.de/zih/dienste/service-katalog/zugangsvoraussetzung), welcher auch zur Nutzung von Matrix berechtigt.

Die Förderation mit den Matrix-Servern anderer wissenschaftlicher oder zivilgesellschaftlicher Institutionen ist jedoch in Kürze möglich (analog zur bestehenden E-Mail-Föderation). Beispiel-Server, mit denen jetzt schon kommuniziert werden kann sind:

* [TU Freiberg](https://matrix.tu-freiberg.de/) inkl. [Doku](https://tu-freiberg.de/en/urz/dienste/chat)

* [TU Chemnitz](https://matrix.tu-chemnitz.de) inkl. [Doku](https://www.tu-chemnitz.de/urz/groupware/chat/doku/)

* [Hochschule Darmstadt](https://chat.fbi.h-da.de) inkl. [Doku](https://its.h-da.io/element-docs/)

* [Hochschule Zittau-Görlitz](https://matrix.hszg.de) inkl. [Doku](https://zfe.hszg.de/das-zfe/aktuelle-entwicklungen/matrix)

* [HMT Leipzig](https://matrix.hmt-leipzig.de)

* [Uni Kiel](https://riot.fs-infmath.uni-kiel.de) inkl. [Doku](https://www.fs-infmath.uni-kiel.de/wiki/Technische_Dienste)

* [Uni Hamburg](http://uni-hamburg.de/)

* [Uni Bremen](https://element.stugen.de/#/welcome)

* [TU Berlin](https://chat.tu-berlin.de/) inkl. [Doku](https://www.innocampus.tu-berlin.de/projekte/matrixinnocampus/)

* [Humboldt Uni Berlin](https://element.hu-berlin.de/) inkl. [Doku](https://www.digitale-lehre.hu-berlin.de/de/lehr-und-lernlandschaft/element)

* [TU München](https://matrix.tum.de) inkl. [Doku](https://wiki.in.tum.de/Informatik/Helpdesk/RIOT)

* [Uni Hannover](https://matrix.uni-hannover.de) inkl. [Doku](https://www.luis.uni-hannover.de/de/services/kommunikation/matrix-messenger/)

* [Uni Osnabrück](https://chat.virtuos.uni-osnabrueck.de/#/welcome) inkl. [Doku](https://www.rz.uni-osnabrueck.de/homeoffice/riot.html)

* [Uni Bielefeld](https://uni-bielefeld.de/teamchat2)

* [Bauhaus-Universität Weimar](https://matrix.bau-ha.us) inkl. [Doku](https://m18.uni-weimar.de/stuko/referate/digitale-infrastruktur)

* [RWTH Aachen](https://riot.comsys.rwth-aachen.de/)

* [Ruhr Universität Bochum](https://riot.rub.de/) inkl. [Doku](https://www.it-services.ruhr-uni-bochum.de/services/issi/element.html.de)

* [Uni Bonn](https://element.matrix.informatik.uni-bonn.de/)

* [Uni Heidelberg](https://matrix-im.uni-heidelberg.de/) inkl. [Doku](https://www.urz.uni-heidelberg.de/en/heichat)

* [Karlsruher Institut für Technologie (KIT)](https://dsn.tm.kit.edu)

* [Uni Augsburg](https://element.physik.uni-augsburg.de/#/welcome) inkl. [Doku](https://www.uni-augsburg.de/de/fakultaet/mntf/physik/facilities/itservices/elequick/)

* [Uni Stuttgart](https://chat.stuvus.de/) inkl. [Doku](https://wiki.stuvus.uni-stuttgart.de/display/ITKB/Matrix+Messenger)


Explizit für Studierende:

* [StudiChat](https://chat.studichat.de/#/welcome) (für alle)

* [Fachschaften](https://matrix.fachschaften.org/) (für Fachschaften)

Weitere europäische Hochschulen:

* [ETH Zürich](https://element.phys.ethz.ch/) inkl. [Doku](https://readme.phys.ethz.ch/chat/)

* [Universität Innsbruck](https://chat.uibk.ac.at/) inkl. [Doku](https://www.uibk.ac.at/zid/anleitungen/chat/)

* [University for Business and Technology, Kosovo](https://ubt-uni.net/)

Kartendarstellung der Hochschulen und Universitäten mit einem Matrix-Dienst: 

<object data="/images/federation_map.svg" type="image/svg+xml" style="width: 600px; max-width: 100%"></object>

Für die zivilgesellschaftliche Nutzung des Protokolls Matrix gibt es hier eine Liste an öffentlichen Heimservern, die auch von Kolleg:innen genutzt werden können, falls ihre Institution noch keinen Matrix-Server anbietet:

[https://austinhuang.me/matrix-homeservers.html](https://austinhuang.me/matrix-homeservers.html)

[https://www.hello-matrix.net/public_servers.php](https://www.hello-matrix.net/public_servers.php)

[https://publiclist.anchel.nl/](https://publiclist.anchel.nl/)

[https://fediverse.blog/~/FossMessenger/matrix-server](https://fediverse.blog/~/FossMessenger/matrix-server)

## Datenschutzerklärung

Datenschutzerklärung: [Link]({{< relref "privacy/_index.md" >}})

## Impressum

Impressum: [Link]({{< relref "imprint/_index.md" >}})

