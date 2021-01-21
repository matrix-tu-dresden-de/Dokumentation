---
title: "Erste Schritte"
date: 2020-08-02T21:26:25+02:00
chapter: true
draft: false
weight: 2
---

# Erste Schritte - Wie kann Matrix genutzt werden?

Mitgliedern und Angehörigen der TU Dresden (selbstverständlich auch Studierenden) wird unter Einhaltung der einschlägigen gesetzlichen und rechtlichen Bestimmungen zum Datenschutz und zur IT-Sicherheit ermöglicht, mittels ihres **ZIH-Logins** mit Angehörigen dieser und anderer Universitäten sowie weiteren Matrix-Nutzenden (bspw. akademischen Partner:innen) per Chat sowie Audio-/Video-Telefonie zu
kommunizieren.

{{% notice tip %}}
Wir empfehlen die Nutzung des Element Desktopclients, weil so viele Probleme, die bei dem Nutzen der Verschlüsselung entstehen können, so vermieden werden.
{{% /notice %}}

Downloads für: {{% button href="https://packages.riot.im/desktop/install/win32/x64/Element%20Setup.exe" icon="fas fa-download" %}}Windows{{% /button %}} {{% button href="https://packages.riot.im/desktop/install/macos/Element.dmg" icon="fas fa-download" %}}macOS{{% /button %}} {{% button href="/clients/install_linux" icon="fas fa-download" %}}Linux{{% /button %}}

Nach einer Desktop-Installation ist darauf zu achten, den bestehenden Account mit dem ZIH-Login zu nutzen, und keinen neuen Account auf einem anderen Server zu erstellen. Hier am Beispiel von Element:

![Markierter Anmeldebutton im Element Matrixclient](/images/01_Login_de.png)

Dies wird durch Klick auf **Ändern** realisiert. Dann landet man nicht versehentlich auf einem falschen Server...

![Anmeldeseite mit Fokus auf dem Homeserver ändern Button](/images/02_Change-Homeserver_de.png)

Nun kann man manuell die Angabe des Heimservers durchführen: https://matrix.tu-dresden.de

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

Matrix verschlüsselt nicht nur die Transporte von und zu dem Heimserver (im Rechenzentrum der TU Dresden) sondern erlaubt auch die Nutzung von Ende-zu-Ende-Verschlüsselung (E2EE). Hierzu müssen kryptografische Schlüssel zwischen allen Geräten ausgetauscht werden, die sich Ende-zu-Ende-verschlüsselt schreiben möchten. Diese technische Notwendigkeit klingt und ist kompliziert, ist inzwischen für die Anwendenden sehr bequem geworden. Die vielen kryptografischen Schlüssel werden vom Client erstellt auf dem jeweiligen Gerät gespeichert. Sollte dies bspw. ein Tab in einem Browser sein, besteht die Gefahr, dass dieser Tab einmal unbeabsichtigt geschlossen wird. Dann sind alle verschlüsselten Inhalte nicht mehr lesbar. Damit dies nicht geschieht, wird eine Schlüsselsicherung auf dem Heimserver der TU Dresden angeboten, auf der (mit einer Sicherheitsphrase (bzw. daraus errechenbaren Sicherheitsschlüssel) geschützt) alle kryptografischen Schlüssel verschlüsselt abgelegt sind.

{{% notice info %}}
Es wird dringend empfohlen, diese Schlüsselsicherung zu nutzen (mit einer sicheren Sicherheitsphrase, welche NICHT Ihr ZIH-Passwort ist) und am Punkt [Weitere wichtige Einstellungen]({{< relref "_index.md#weitere-wichtige-einstellungen" >}}) weiterlesen!
{{% /notice %}}

   ![Screenshot der Aufforderung eine Sicherheitsphrase einzugeben](/images/01_Restore-Session_de.png)

Sollten Sie dies jetzt überspringen, sähe der nächste Bildschirm so aus:

   ![Bestätigung des Überspringes der Eingabe einer Sicherheitsphrase](/images/03_Cancel-Restore_de.png)

Die Schlüsselsicherung wird dringend empfohlen, um sorgenfrei Ende-zu-Ende-Verschlüsselung nutzen zu können. Daher wird auch nach einem weiteren Überspringen in einem kleineren Tooltip zur Einrichtung der Verschlüsselung aufgefordert:

   ![Chatansicht mit der Anzeige eines Tooltips, Verschlüsselung einzurichten. Markierung des bestätigen Feldes](/images/04_Notification_de.png)

Sollten Sie dies auch hier auslassen wird Ihnen eine letzte Warnung bei einem bewussten Abmelden angezeigt. Wenn spätestens hierbei keine Schlüsselsicherung eingerichtet wird, kann später auf ggf. schon stattgefundene verschlüsselte Gespräche nicht mehr zugegriffen werden. Sollte der Tab geschlossen werden, entspricht dies ggf. ebenfalls einem Abmelden.

   ![Abfrage, ob Nachrichten verschlüsselt werden sollen](/images/05_Logout-Notify_de.png)


## Nutzung des Webclients

Eine Anleitung für den Webclient finden Sie unter: [clients -> browser]({{< relref "clients/browser.md" >}})

Eine Registrierung von Accounts (wie vllt. von anderen Matrix-Servern bekannt) ist hier an der TU Dresden nicht möglich, da den Dienst ausschließlich Personen mit ZIH-Login nutzen können. Die TU Dresden ist kein Kommunikationsdiensteanbieter.

Für wissenschaftliche Kooperationen mit Kolleg:innen ohne ZIH-Account besteht die Möglichkeit zur [Beantragung eines ZIH-Gast-Accounts](https://tu-dresden.de/zih/dienste/service-katalog/zugangsvoraussetzung), welcher auch zur Nutzung von Matrix berechtigt.

Die Förderation mit den Matrix-Servern anderer wissenschaftlicher oder zivilgesellschaftlicher Institutionen ist jedoch in Kürze möglich (analog zur bestehenden E-Mail-Föderation). Beispiel-Server, mit denen jetzt schon kommuniziert werden kann sind:

* [TU München](https://tum.de)

* [Uni Hamburg](http://uni-hamburg.de/)

* [TU Berlin](http://matrix.tu-berlin.de/)

* [Uni Heidelberg](https://uni-heidelberg.de/)

* [Uni Bochum](http://ruhr-uni-bochum.de)

* [TU Freiberg](https://tu-freiberg.de)

* [TU Chemnitz](http://tu-chemnitz.de)

* [Hochschule Weimar](http://bau-ha.us)

* [ETH Zürich](https://readme.phys.ethz.ch/chat/)

* [University for Business and Technology, Kosovo](https://ubt-uni.net/)

Für die zivilgesellschaftliche Nutzung des Protkolls Matrix gibt es hier eine Liste an öffentlichen Heimservern, die auch von Kolleg:innen genutzt werden können, falls ihre Institution noch keinen Matrix-Server anbietet:
[https://www.hello-matrix.net/public_servers.php](https://www.hello-matrix.net/public_servers.php)

Datenschutzerklärung: https://matrix.tu-dresden.de/datenschutz.html

Impressum: https://matrix.tu-dresden.de/impressum.html

