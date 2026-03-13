---
title: "Erste Schritte"
date: 2020-08-02T21:26:25+02:00
chapter: true
draft: false
weight: 2
---

# Erste Schritte mit Matrix

## Matrix-Login mit TUD-Account

Mitgliedern und Angehörigen der TU Dresden (insbesondere auch Studierenden) wird durch Matrix ermöglicht, mittels ihres **TUD-Logins** mit Angehörigen dieser und anderer Hochschulen und Universitäten sowie weiteren Matrix-Nutzenden (beispielsweise akademischen Partner:innen) per Chat sowie Audio-/Video-Telefonie zu kommunizieren.

Die Kommunikation erfolgt über einen sogenannten Client. Es steht eine [Vielzahl verschiedener Clients](https://matrix.org/clients/) zur Auswahl. Der bekannteste Client ist Element (früher Riot). Neben mobilen Versionen für Android und IOS bieten wir Element als Web-Anwendung unter [chat.tu-berlin.de](https://chat.tu-berlin.de) an. Element steht aber auch als Desktop-Anwendung zum [Download](https://element.io/download) bereit.

{{% notice tip %}}
Wir empfehlen die Nutzung des Element Desktop-Clients, weil so zahlreiche Probleme, die bei dem Nutzen der Verschlüsselung entstehen können, vermieden werden können.
{{% /notice %}}

{{% notice warning %}}
Bei einer Installation von Element Desktop und den mobilen Apps für Android und IOS ist darauf zu achten, dass die Anmeldung mit dem TUB-Account auf dem lokalen Homeserver der TU Berlin erfolgt und kein neuer Account auf einem anderen Homeserver erstellt wird.
{{% /notice %}}

Dazu muss man im Client die URL des lokalen Homeservers eintragen. Hier am Beispiel von Element-Desktop:

![Markierter Anmeldebutton im Element Matrixclient](/images/01_Login_de.png)

Um sich auf dem Homeserver der TU Berlin anzumelden, klickt man zunächst auf **Anmelden** und anschließend auf **Bearbeiten**.

![Anmeldeseite mit Fokus auf dem Homeserver ändern Button](/images/02_Change-Homeserver_de.png)

Nun kann man manuell *tu-dresden.de* als Homeserver angeben.

![Eingabefeld zum Ändern des Homeservers mit der Eingabe matrix.tu-dresden.de](/images/03_Set-Homeserver_de.png)

Anschließend ist der einmalige Login mit TUD-Login (= ZIH-Login) und TUD-Passwort (= ZIH-Passwort) durchzuführen:
Dropdown-Menü „Anmelden mit:“ sollte auf „Benutzername“ belassen werden. Dann sind folgende Eingaben zu tätigen:

**Benutzername: TUD-Login**  ( = ZIH-Login, nur das Login-Kürzel, keine E-Mail-Adresse!)

**Passwort: TUD-Passwort** (= ZIH-Passwort)

Ein alternativer Login, bspw. über die E-Mail-Adresse ist **NICHT** beim ersten, initialen, Anmelden möglich, erst ab dem zweiten Einloggen.

Es folgt nach dem Erstlogin auch keine E-Mail / Bestätigungsmail.





![Loginfenster mit Aufforderung TUB-Login und Passwort einzugeben](/images/04_Username_de.png)

Analog zu E-Mail-Adressen ergibt sich eine Matrix-Adresse, über die man von anderen Nutzenden zur Kommunikation eingeladen werden kann:

<p style="text-align: center; font-style: italic;">@&lt;tu_login&gt;:matrix.tu-berlin.de</p>

## Einrichtung der Schlüsselsicherung

Nach der ersten Anmeldung werden Sie nach einiger Zeit dazu aufgefordert die Schlüsselsicherung einzurichten und andere wichtige Einstellungen vorzunehmen.

{{% notice info %}}
Es wird dringend empfohlen sich die Zeit zu nehmen und die Schlüsselsicherung einzurichten. Andernfalls kann es passieren, dass Nachrichten nicht mehr entschlüsselt werden können und so verloren gehen.
{{% /notice %}}

Matrix verschlüsselt nicht nur die Daten zwischen den Clients und dem Homeserver (im Rechenzentrum der TU Dresden) sondern erlaubt auch die Nutzung von Ende-zu-Ende-Verschlüsselung (E2EE). Hierzu müssen kryptografische Schlüssel zwischen allen beteiligten Geräten ausgetauscht werden. Obwohl diese technische Notwendigkeit kompliziert klingt und im Hintergrund auch ist, ist sie inzwischen für die Anwendenden sehr bequem geworden. Die vielen kryptografischen Schlüssel werden vom Client erstellt auf dem jeweiligen Gerät gespeichert. Sollte dies beispielsweise ein Tab in einem Browser sein, besteht die Gefahr, dass dieser Tab einmal unbeabsichtigt geschlossen wird. Dann sind verschlüsselten Inhalte unter Umständen nicht mehr lesbar. Damit dies nicht geschieht, wird eine Schlüsselsicherung auf dem Homeserver der TU Dresden angeboten, auf der (mit einer Sicherheitsphrase bzw. daraus errechenbaren Sicherheitsschlüssel geschützt) alle kryptografischen Schlüssel (verschlüsselt) abgelegt sind.

![Aufforderung den Sicherheitsschlüssel zu generieren oder eine Sicherheitsphrase einzugeben](/images/11_Setup-Key_de.png)
![Aufforderung eine Passwort für die Schlüsselsicherung einzugeben](/images/12_Enter-Key_de.png)

Bei der Wahl der Sicherheitsphrase ist darauf zu achten, dass diese **nicht** Ihrem TUD-Passwort entsprechen darf! Alternativ können Sie sich statt der Sicherheitsphrase auch einen Sicherheitsschlüssel generieren lassen, welcher den selben Zweck wie die Sicherheitsphrase erfüllt. Weiterhin wird der Sicherheitsschlüssel immer zusätzlich zur Sicherheitsphrase erstellt und sollte als Notfallschlüssel sicher und wieder auffindbar verwahrt werden (z.B. Abspeichern als .txt-Datei und Ausdrucken).

![Anzeige des Sicherheitsschlüssel zum abschreiben oder wegspeichern](/images/13_Present-Key_de.png)

Meldet man sich nun von einem anderen Gerät beziehungsweise mit einem anderen Client an, wird man dazu aufgefordert die Sitzung zu verifizieren. Ist man noch mit einem weiteren Client angemeldet, kann die Verifikation über dieses Gerät erfolgen. Andernfalls ist man auf den Sicherheitsschlüssel oder die Sicherheitsphrase angewiesen.

![Screenshot der Aufforderung eine Sicherheitsphrase einzugeben](/images/01_Restore-Session_de.png)

Sollte die Schlüsselsicherung nicht eingerichtet worden sein, kann nach einer Abmeldung nicht auf verschlüsselte Nachrichten zugegriffen werden. Auch das Schließen eines Browser-Tabs kann unter ungünstigen Umständen zu einer Abmeldung des Clients vom Homeserver führen.

![Bestätigung des Überspringens der Eingabe einer Sicherheitsphrase](/images/03_Cancel-Restore_de.png)

Vermeiden Sie diese Situation durch eine eingerichtete Schlüsselsicherung!

## Konfiguration des Clients

Durch [weitere wichtige Einstellungen]({{< relref "settings/_index.md" >}}) können Sie Ihren Client an Ihre Bedürfnisse anpassen und so ihr Matrix-Erlebnis verbessern!

## Matrix-Login ohne TUD-Account

Eine Registrierung von Accounts (wie vielleicht von anderen Matrix-Servern bekannt) ist an der TU Dresden nicht möglich. Der Dienst kann ausschließlich von Angehörigen der TU Dresden mit TUD-Login genutzt werden.

Es ist jedoch möglich mit Nutzenden anderer Matrix-Homeserver von verschiedenen wissenschaftlichen und zivilgesellschaftlichen Institutionen zu kommunizieren. Dieses Feature nennt sich Föderation (das Prinzip ist ähnlich zu dem E-Mail System: E-Mails können beispielsweise von den Servern der TU Dresden an die Sever der TU Berlin geschickt werden).

Auf öffentlichen Homeservern (wie zum Beispiel dem von [matrix.org](https://app.element.io/)) kann sich jede Person einen Account anlegen. Wir bitten externe, die über Matrix mit Angehörigen der TU Dresden kommunizieren wollen, diese Möglichkeit zu nutzen. Eine Liste mit weiteren öffentlichen Homeservern ist auf [hello-matrix.net](https://www.hello-matrix.net/public_servers.php) verfügbar.

Folgende deutsche Hochschulen verfügen über einen eigenen Homeserver:

* [TU Freiberg](https://matrix.tu-freiberg.de/) inkl. [Doku](https://tu-freiberg.de/en/urz/dienste/chat)

* [TU Chemnitz](https://matrix.tu-chemnitz.de) inkl. [Doku](https://www.tu-chemnitz.de/urz/groupware/chat/doku/)

* [Hochschule Darmstadt](https://chat.fbi.h-da.de) inkl. [Doku](https://its.h-da.io/element-docs/)

* [Hochschule Zittau-Görlitz](https://matrix.hszg.de) inkl. [Doku](https://zfe.hszg.de/das-zfe/aktuelle-entwicklungen/matrix)

* [HMT Leipzig](https://chat.hmt-leipzig.de)

* [Uni Hamburg](http://uni-hamburg.de/)

* [Uni Bremen](https://element.stugen.de/#/welcome)

* [TU Berlin](https://chat.tu-berlin.de/) inkl. [Doku](https://www.innocampus.tu-berlin.de/projekte/matrixinnocampus/)

* [Humboldt Uni Berlin](https://element.hu-berlin.de/) inkl. [Doku](https://www.digitale-lehre.hu-berlin.de/de/lehr-und-lernlandschaft/element)
* [Universität der Künste Berlin](https://medienhaus.udk-berlin.de/classroom)

* [TU München](https://matrix.tum.de) inkl. [Doku](https://wiki.in.tum.de/Informatik/Helpdesk/RIOT)

* [Uni Hannover](https://matrix.uni-hannover.de) inkl. [Doku](https://www.luis.uni-hannover.de/de/services/kommunikation/matrix-messenger/)

* [Uni Osnabrück](https://element.uni-osnabrueck.de) inkl. [Doku](https://digitale-lehre.virtuos.uni-osnabrueck.de/eintrag/instant-messenger-element/)

* [Uni Bielefeld](https://uni-bielefeld.de/teamchat2)

* [Bauhaus-Universität Weimar](https://chat.uni-weimar.de/) inkl. [Doku](https://chat.uni-weimar.de/docs/matrix/)

* [RWTH Aachen](https://riot.comsys.rwth-aachen.de/)

* [Ruhr Universität Bochum](https://riot.rub.de/) inkl. [Doku](https://www.it-services.ruhr-uni-bochum.de/services/issi/element.html.de)

* [Uni Bonn](https://element.matrix.informatik.uni-bonn.de/)

* [Uni Heidelberg](https://matrix-im.uni-heidelberg.de/) inkl. [Doku](https://www.urz.uni-heidelberg.de/en/heichat)

* [Karlsruher Institut für Technologie (KIT)](https://matrix.kit.edu/)

* [Uni Augsburg](https://element.physik.uni-augsburg.de/#/welcome) inkl. [Doku](https://www.uni-augsburg.de/de/fakultaet/mntf/physik/facilities/itservices/elequick/)

* [Uni Stuttgart](https://chat.stuvus.de/) inkl. [Doku](https://wiki.stuvus.uni-stuttgart.de/display/ITKB/Matrix+Messenger)

* [Hochschule Bremerhaven](https://matrix.hs-bremerhaven.de/)

* [TU Darmstadt](https://element.matrix.tu-darmstadt.de)

* [Philipps-Universität Marburg](https://matrix.uni-marburg.de/)

* [TU Braunschweig](https://chat.tu-bs.de/)

* [Hochschule Furtwangen](https://matrix.hs-furtwangen.de/) inkl. [Doku](https://howto.hs-furtwangen.de/hfu-chat/)

* [Friedrich-Alexander-Universität Erlangen-Nürnberg](https://chat.fau.de/) inkl. [Doku](https://www.rrze.fau.de/serverdienste/matrix/)

* [Friedrich-Schiller-Universität Jena](https://chat.uni-jena.de/) inkl. [Doku](https://wiki.uni-jena.de/display/URZ010SD/Chatten+mit+Matrix)

* [Albert-Ludwigs-Universität Freiburg](https://matrix.uni-freiburg.de/)

* [Hochschule Stralsund](https://matrix.hochschule-stralsund.de) inkl. [Doku](https://matrix.hochschule-stralsund.de/doc/)

* [Technische Hochschule Mittelhessen](https://element.thm.de) inkl. [Doku](https://go.thm.de/thmconnect)

Homeserver explizit für Studierende:

* [StudiChat](https://chat.studichat.de/#/welcome) (für alle)

* [Fachschaften](https://matrix.fachschaften.org/) (für Fachschaften)

Weitere europäische Hochschulen mit einem eigenen Homeserver:

* [ETH Zürich](https://element.phys.ethz.ch/) inkl. [Doku](https://readme.phys.ethz.ch/chat/)

* [Universität Innsbruck](https://chat.uibk.ac.at/) inkl. [Doku](https://www.uibk.ac.at/zid/anleitungen/chat/)

* [University for Business and Technology, Kosovo](https://ubt-uni.net/)

* [Karl-Franzens-Universität Graz](https://chat.uni-graz.at/)

* [University of Oxford](https://chat.cs.ox.ac.uk) inkl. [Doku](https://users.ox.ac.uk/~ball5903/oums/)

* [École polytechnique fédérale de Lausanne](https://element.epfl.ch/)

Kartendarstellung der Hochschulen und Universitäten mit einem Matrix-Dienst:

<object data="/images/federation_map.svg" type="image/svg+xml" style="width: 600px; max-width: 100%"></object>

<!--Für die zivilgesellschaftliche Nutzung des Protokolls Matrix gibt es hier eine Liste an öffentlichen Homeservern, die auch von Kolleg:innen genutzt werden können, falls ihre Institution noch keinen Matrix-Server anbietet:

[https://austinhuang.me/matrix-homeservers.html](https://austinhuang.me/matrix-homeservers.html)

[https://www.hello-matrix.net/public_servers.php](https://www.hello-matrix.net/public_servers.php)

[https://publiclist.anchel.nl/](https://publiclist.anchel.nl/)

[https://fediverse.blog/~/FossMessenger/matrix-server](https://fediverse.blog/~/FossMessenger/matrix-server)-->

## Datenschutzerklärung

Datenschutzerklärung: [Link]({{< relref "privacy/_index.md" >}})

## Impressum

Impressum: [Link]({{< relref "imprint/_index.md" >}})
