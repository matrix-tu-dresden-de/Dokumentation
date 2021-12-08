---
title: "First steps"
date: 2020-08-02T21:26:25+02:00
chapter: true
draft: false
weight: 2
---

# First steps - How to use Matrix?

## Matrix-Login with ZIH account

Members and members of the TU Dresden (of course also students) can use their **ZIH login** to communicate with members of the TU Dresden and other universities and other Matrix users (e.g. academic partners) via chat and audio/video telephony in compliance with the relevant legal and regulatory provisions on data protection and IT security.

{{% notice tip %}}
We recommend using the Element desktop client, because this avoids most problems users have with Matrix, e.g. end to end encryption.
{{% /notice %}}

Downloads for: {{% button href="https://packages.riot.im/desktop/install/win32/x64/Element%20Setup.exe" icon="fas fa-download" %}}Windows{{% /button %}} {{% button href="https://packages.riot.im/desktop/install/macos/Element.dmg" icon="fas fa-download" %}}macOS{{% /button %}} {{% button href="/clients/install_linux" icon="fas fa-download" %}}Linux{{% /button %}}

After a desktop installation, make sure to use the existing account with the ZIH login and not to create a new account on another server. Here the example of Element:

![Selected login button in the element matrix client](/images/01_Login_en.png)

This is done by clicking on **Change**. Then you will not accidentally end up on the wrong server...

![Change login page with focus on the homeserver button](/images/02_Change-Homeserver_en.png)

Now you can manually specify the home server: tu-dresden.de

![Input field to change the home server with the input matrix.tu-dresden.de](/images/03_Set-Homeserver_en.png)

Afterwards the login with ZIH login and ZIH password must be carried out:

The drop-down menu "Log in with:" should be left at "User name". Then the following entries must be made:

**Username: ZIH-Login** (only the ZIH-Login, no e-mail address!)

**Password: ZIH-Password**

An alternative login, e.g. using the e-mail address, is **NOT** possible during the first, initial login, only after the second login.

After the first login there is also no e-mail / confirmation mail.

Analogous to e-mail addresses, this results in matrix addresses with the following structure:

@ZIH-Login:tu-dresden.de

![Login window with request to enter ZIH login and password](/images/04_Username_en.png)

## Convenient use of end-to-end encryption (E2EE)

Matrix not only encrypts transports to and from the home server (in the data center of TU Dresden) but also allows the use of end-to-end encryption (E2EE). For this, cryptographic keys have to be exchanged between all devices that want to write end-to-end encrypted. This technical necessity sounds and is complicated, but in the meantime it has become very convenient for the users. The many cryptographic keys created by the client are stored on the respective device. If this is a tab in a browser, for example, there is a risk that this tab will be closed unintentionally. Then all encrypted contents are no longer readable. To prevent this from happening, a key protection is offered on the home server of the TU Dresden, on which (protected with a security phrase (or security key that can be calculated from it) all cryptographic keys are stored encrypted. 
   
{{% notice info %}}
It is highly recommended to use this key backup (with a secure security phrase which is NOT your ZIH password)!
{{% /notice %}}
   
![Prompt to generate the security key or enter a security phrase](/images/11_Setup-Key_en.png)
![Prompt to enter a password for the key backup](/images/12_Enter-Key_en.png)
Alternatively, instead of the security phrase, you can also have a security key generated that serves the same purpose as the security phrase. Furthermore, the security key is generated in addition to the security phrase and should be kept safe and retrievable as an emergency key (e.g. save it as .txt file AND print it out) 
![Display of the security key to write or save away](/images/13_Present-Key_en.png) 

[Other important settings]({{< relref "settings/_index.en.md" >}}) may improve your Matrix experience!


## Requests to setup the key backup

![Screenshot of the prompt to enter a security phrase](/images/01_Restore-Session_en.png)

If you skipped the request to setup the key backup, the next screen would look like this:

![Confirmation of skipping the input of a security phrase](/images/03_Cancel-Restore_en.png)

Key protection is highly recommended for worry-free end-to-end encryption. For this reason, a smaller tooltip will prompt you to set up the encryption even after you skip further:
   
![Chat view showing a tooltip to set up encryption. Marking the confirm field](/images/04_Notification_en.png)

If you omit this here as well, you will get a last warning if you log off consciously. If no key backup is set up at the latest, encrypted calls that may have already taken place cannot be accessed later. If the tab is closed, this also corresponds to a logout.
   
![Query if messages should be encrypted](/images/05_Logout-Notify_en.png)

Avoid this situation by setting up a key backup!

## Matrix-Login without ZIH account

A registration of accounts (as known from other matrix servers) is not possible here at the TU Dresden, because only persons with ZIH login can use the service. The TU Dresden is not a communication service provider. 

For scientific cooperations with colleagues without a ZIH account there is the possibility to [apply for a ZIH guest account](https://tu-dresden.de/zih/dienste/service-katalog/zugangsvoraussetzung), which also entitles to use Matrix.

However, the federation with the Matrix servers of other scientific or civil society institutions will soon be possible (analogous to the existing e-mail federation). Example servers with which communication is already possible are:

* [TU Freiberg](https://matrix.tu-freiberg.de/) incl. [Docu](https://tu-freiberg.de/en/urz/dienste/chat)

* [TU Chemnitz](https://matrix.tu-chemnitz.de) incl. [Docu](https://www.tu-chemnitz.de/urz/groupware/chat/doku/)

* [Hochschule Darmstadt](https://chat.fbi.h-da.de) incl. [Doku](https://its.h-da.io/element-docs/)

* [Hochschule Zittau-Görlitz](https://matrix.hszg.de) incl. [Docu](https://zfe.hszg.de/das-zfe/aktuelle-entwicklungen/matrix)

* [HMT Leipzig](https://matrix.hmt-leipzig.de)

* [Uni Kiel](https://riot.fs-infmath.uni-kiel.de) incl. [Docu](https://www.fs-infmath.uni-kiel.de/wiki/Technische_Dienste)

* [Uni Hamburg](http://uni-hamburg.de/)

* [Uni Bremen](https://element.stugen.de/#/welcome)

* [TU Berlin](https://chat.tu-berlin.de/) incl. [Docu](https://www.innocampus.tu-berlin.de/projekte/matrixinnocampus/)

* [Humboldt Uni Berlin](https://element.hu-berlin.de/) incl. [Docu](https://www.digitale-lehre.hu-berlin.de/de/lehr-und-lernlandschaft/element)

* [TU München](https://matrix.tum.de) incl. [Docu](https://wiki.in.tum.de/Informatik/Helpdesk/RIOT)

* [Uni Hannover](https://matrix.uni-hannover.de) incl. [Docu](https://www.luis.uni-hannover.de/de/services/kommunikation/matrix-messenger/)

* [Uni Osnabrück](https://chat.virtuos.uni-osnabrueck.de/#/welcome) incl. [Docu](https://www.rz.uni-osnabrueck.de/homeoffice/riot.html)

* [Uni Bielefeld](https://uni-bielefeld.de/teamchat2)

* [Bauhaus-Universität Weimar](https://matrix.bau-ha.us) incl. [Docu](https://m18.uni-weimar.de/stuko/referate/digitale-infrastruktur)

* [RWTH Aachen](https://riot.comsys.rwth-aachen.de/)

* [Ruhr Universität Bochum](https://riot.rub.de/) incl. [Docu](https://www.it-services.ruhr-uni-bochum.de/services/issi/element.html.de)

* [Uni Bonn](https://element.matrix.informatik.uni-bonn.de/)

* [Uni Heidelberg](https://matrix-im.uni-heidelberg.de/) incl. [Docu](https://www.urz.uni-heidelberg.de/en/heichat)

* [Karlsruher Institut für Technologie (KIT)](https://dsn.tm.kit.edu)

* [Uni Augsburg](https://element.physik.uni-augsburg.de/#/welcome) incl. [Docu](https://www.uni-augsburg.de/de/fakultaet/mntf/physik/facilities/itservices/elequick/)

* [Uni Stuttgart](https://chat.stuvus.de/) incl. [Docu](https://wiki.stuvus.uni-stuttgart.de/display/ITKB/Matrix+Messenger)


Explizit für Studierende:

* [StudiChat](https://chat.studichat.de/#/welcome) (für alle)

* [Fachschaften](https://matrix.fachschaften.org/) (für Fachschaften)

Weitere europäische Hochschulen:

* [ETH Zürich](https://element.phys.ethz.ch/) incl. [Docu](https://readme.phys.ethz.ch/chat/)

* [Universität Innsbruck](https://chat.uibk.ac.at/) incl. [Docu](https://www.uibk.ac.at/zid/anleitungen/chat/)

* [University for Business and Technology, Kosovo](https://ubt-uni.net/)


<object data="/images/federation_map.svg" type="image/svg+xml" style="width: 600px; max-width: 100%"></object>


For civil use of the Matrix protocol, here is a list of public home servers that can also be used by Kolleg:innen if their institution does not yet offer a Matrix server:

[https://austinhuang.me/matrix-homeservers.html](https://austinhuang.me/matrix-homeservers.html)

[https://www.hello-matrix.net/public_servers.php](https://www.hello-matrix.net/public_servers.php)

[https://publiclist.anchel.nl/](https://publiclist.anchel.nl/)

[https://fediverse.blog/~/FossMessenger/matrix-server](https://fediverse.blog/~/FossMessenger/matrix-server)


## Privacy policy

Privacy policy: [Link]({{< relref "privacy/_index.en.md" >}})

## Imprint

Imprint: [Link]({{< relref "imprint/_index.en.md" >}})
