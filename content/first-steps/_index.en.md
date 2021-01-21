---
title: "First steps"
date: 2020-08-02T21:26:25+02:00
chapter: true
draft: false
weight: 2
---

# First steps - How to use Matrix?

Members and members of the TU Dresden (of course also students) can use their **ZIH login** to communicate with members of the TU Dresden and other universities and other Matrix users (e.g. academic partners) via chat and audio/video telephony in compliance with the relevant legal and regulatory provisions on data protection and IT security.
communicate.

{{% notice tip %}}
We recommend using the Element desktop client, because this avoids most problems users have with Matrix, e.g. end to end encryption.
{{% /notice %}}

Downloads for: {{% button href="https://packages.riot.im/desktop/install/win32/x64/Element%20Setup.exe" icon="fas fa-download" %}}Windows{{% /button %}} {{% button href="https://packages.riot.im/desktop/install/macos/Element.dmg" icon="fas fa-download" %}}macOS{{% /button %}} {{% button href="/clients/install_linux" icon="fas fa-download" %}}Linux{{% /button %}}

After a desktop installation, make sure to use the existing account with the ZIH login and not to create a new account on another server. Here the example of Element:

![Selected login button in the element matrix client](/images/01_Login_en.png)

This is done by clicking on **Change**. Then you will not accidentally end up on the wrong server...

![Change login page with focus on the homeserver button](/images/02_Change-Homeserver_en.png)

Now you can manually specify the home server: https://matrix.tu-dresden.de

![Input field to change the home server with the input matrix.tu-dresden.de](/images/03_Set-Homeserver_en.png)

Afterwards the login with ZIH login and ZIH password must be carried out:

The drop-down menu "Log in with:" should be left at "User name". Then the following entries must be made:

**Username: ZIH-Login** (only the ZIH-Login, no e-mail address!)

**Password: ZIH password**

An alternative login, e.g. using the e-mail address, is **NOT** possible during the first, initial login, only after the second login.

After the first login there is also no e-mail / confirmation mail.

Analogous to e-mail addresses, this results in matrix addresses with the following structure:

@ZIH-Login:tu-dresden.de

![Login window with request to enter ZIH login and password](/images/04_Username_en.png)

## Convenient use of end-to-end encryption (E2EE)

Matrix not only encrypts transports to and from the home server (in the data center of TU Dresden) but also allows the use of end-to-end encryption (E2EE). For this, cryptographic keys have to be exchanged between all devices that want to write end-to-end encrypted. This technical necessity sounds and is complicated, but in the meantime it has become very convenient for the users. The many cryptographic keys created by the client are stored on the respective device. If this is a tab in a browser, for example, there is a risk that this tab will be closed unintentionally. Then all encrypted contents are no longer readable. To prevent this from happening, a key protection is offered on the home server of the TU Dresden, on which (protected with a security phrase (or security key that can be calculated from it) all cryptographic keys are stored encrypted. 

{{% notice info %}}
It is highly recommended to use this key backup (with a secure security phrase which is NOT your ZIH password) and read on at [Other important settings]({{< relref "_index.en.md#other-important-settings" >}})!
{{% /notice %}}
   
![Screenshot of the prompt to enter a security phrase](/images/01_Restore-Session_en.png)

If you skip this now, the next screen would look like this:
   
![Confirmation of skipping the input of a security phrase](/images/03_Cancel-Restore_en.png)

Key protection is highly recommended for worry-free end-to-end encryption. For this reason, a smaller tooltip will prompt you to set up the encryption even after you skip further:
   
![Chat view showing a tooltip to set up encryption. Marking the confirm field](/images/04_Notification_en.png)

If you omit this here as well, you will get a last warning if you log off consciously. If no key backup is set up at the latest, encrypted calls that may have already taken place cannot be accessed later. If the tab is closed, this also corresponds to a logout.
   
![Query if messages should be encrypted](/images/05_Logout-Notify_en.png)

## Webclient

For using the Webclient, see the manuel under [clients -> browser]({{< relref "clients/browser.en.md" >}})

A registration of accounts (as known from other matrix servers) is not possible here at the TU Dresden, because only persons with ZIH login can use the service. The TU Dresden is not a communication service provider. 

For scientific cooperations with colleagues without a ZIH account there is the possibility to [apply for a ZIH guest account](https://tu-dresden.de/zih/dienste/service-katalog/zugangsvoraussetzung), which also entitles to use Matrix.

However, the federation with the Matrix servers of other scientific or civil society institutions will soon be possible (analogous to the existing e-mail federation). Example servers with which communication is already possible are:

* [TU München](https://tum.de)

* [Uni Hamburg](http://uni-hamburg.de/)

* [Uni Heidelberg](https://uni-heidelberg.de/)

* [Uni Bochum](http://ruhr-uni-bochum.de)

* [TU Freiberg](https://tu-freiberg.de)

* [TU Chemnitz](http://tu-chemnitz.de)

* [Hochschule Weimar](http://bau-ha.us)

* [ETH Zürich](https://readme.phys.ethz.ch/chat/)

* [University for Business and Technology, Kosovo](https://ubt-uni.net/)

For civil use of the Matrix protocol, here is a list of public home servers that can also be used by Kolleg:innen if their institution does not yet offer a Matrix server:
[https://www.hello-matrix.net/public_servers.php](https://www.hello-matrix.net/public_servers.php)
