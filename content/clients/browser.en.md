---
title: "Element Web (Browser)"
date: 2020-07-15T16:46:07+02:00
draft: false
chapter: true
weight: 10
---

# Using the Element webclient
Start here: [https://matrix.tu-dresden.de](https://matrix.tu-dresden.de) 

![Start page of Element Webclient with login button](/images/01_Welcome_en.png)

No registration is necessary, the service can be used immediately by clicking on "Register" on the homepage [https://matrix.tu-dresden.de](https://matrix.tu-dresden.de).

![Login window with request to enter ZIH login and password](/images/02_Login1_en.png)

The drop-down menu "Log in with:" should be left at "User name". Then the following entries must be made:

**Username: ZIH-Login** (only the ZIH-Login, no e-mail address!)

**Password: ZIH password**

An alternative login, e.g. using the e-mail address, is **NOT** possible during the first, initial login, only after the second login.

After the first login there is also no e-mail / confirmation mail.

Analogous to e-mail addresses, this results in matrix addresses with the following structure:

@ZIH-Login:tu-dresden.de

{{% notice warning %}}
If you want to start immediately with a [Matrix Client]({{< relref "../clients" >}}) instead of the above mentioned website (Element Web-App installed at TU Dresden), it is important to change the home server from the usually default matrix.org to https://matrix.tu-dresden.de (shown in the following three screenshots)
{{% /notice %}}

![Change login page with focus on the homeserver Button](/images/02_Login2_en.png)

1. click on change

![input field to change the home server with the input matrix.tu-dresden.de](/images/02_Login3_en.png)

2. mark the preset home server address and remove it

![](/images/02_Login4_en.png)

3. entry of the matrix home server address of the TU Dresden

## Browser settings

### Browser selection

Recommended are the browsers [Firefox](https://www.mozilla.org/de/firefox/new/), [Chromium](https://www.chromium.org/getting-involved/download-chromium), newer versions of MS Edge (based on Chromium). Older or unsuitable browsers may only show a white page.

### NoScript

Many people use script blockers to protect themselves from [Tracking](https://tu-dresden.de/tu-dresden/newsportal/news/datenschutz-beim-website-tracking) and malware in the browser, for example with the addon [NoScript](https://addons.mozilla.org/de/firefox/addon/noscript/). Here you have to make the following settings (for the integration manager, e.g. Jitsi/Etherpad)

![Browser plugin settings NoScript with tu-dresden.de and vector.im selected as trusted script sources](/images/10_Sicherheit2_en.png)

### Cookies

Do you also allow cookies from

- tu-dresden.de
- vector.im (for the integration manager)
