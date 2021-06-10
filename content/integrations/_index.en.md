---
title: "Integrations"
date: 2020-07-02T21:23:01+02:00
draft: false
chapter: true
weight: 80
---

# Use integrations, bridges, bots (e.g. Jitsi)

Integrations/Widgets can be managed via the room information in the upper right corner.

![Add integration button](/images/01_Widgets_en.png)

Here, for example, an etherpad, a jitsi video conference, an RSS bot, etc. can be integrated, i.e. services that are located and run on other servers. Therefore, when using integrations, the JavaScript activity of vector.im (for the integration manager) and other servers (e.g. in the Firefox addon NoScript) must be allowed. Since the widgets are often too small to use the services in their full functionality, widgets can often be opened large in new browser tabs.

In the following videos Prof. Dr. Alexander Lasch presents some possibilities for integrating widgets into matrix rooms for digital teaching:

https://invidious.13ad.de/watch?v=AtkA-sE-9uU

https://invidious.13ad.de/watch?v=D2Pq-NCaVGE

## Jitsi Videoconference

A 1:1 phone call or video within Matrix uses the direct WebRTC connection between both parties. From the 3rd person on, [Jitsi](https://de.wikipedia.org/wiki/Jitsi) is used, a free video conferencing tool (Apache license), which was installed locally at the TU Dresden in the course of the Corona crisis and the reduced availability of DFNconf: https://jitsi.tu-dresden.de

If the video conference call is started via the camera icon in the lower right corner, the Jitsi operated by the TU Dresden is automatically used. In order for Jitsi to be used for the video conference, at least three people must participate in the conference. If only two people participate in the conference, a direct connection will be established.

{{% notice warning %}}
If the jitsi integration is added via the Integration Manager, the jitsi instance of TU Dresden is not used
{{% /notice %}}

Also with Jitsi, opening the widget as a separate tab is useful to use the full functionality (e.g. screen sharing). 

The use of a headset (headphone + microphone) is highly recommended to avoid feedback between sound recording and sound playback. Ideally a headset with a microphone close to the head and not just a headphone and use of the microphone hole on the laptop, which causes noise through it.

The m key mutes your microphone - with this setting you should always start a conference. The space bar switches the microphone on when muting is active (push-to-talk). Since the microphone input levels are all set differently, all hearing participants can adjust the volume of all conference participants individually. Furthermore, the individual video quality can be adjusted. 

For sharing the screen contents (or specific program windows), it may be necessary to adjust the security settings of the operating system (e.g. in MacOS under System Preferences > Security > Privacy > Screen Capture).

Many thanks to Dr. Eike Dohmen ([Professorship of Magnetofluiddynamics, Measurement and Automation Technology](https://tu-dresden.de/ing/maschinenwesen/imd/mfd)) and Prof. Dr. Alexander Lasch ([Professorship of German Linguistics and History of Language](http://tu-dresden.de/gsw/slk/germanistik/gls/)) for tests and hints on the interaction of Matrix and Jitsi.

## Etherpad

The Etherpad widget can be used for collaborative writing or attaching important information to a room.

{{% notice warning %}}
For this purpose, a name must be assigned which must have less than 16 characters!
{{% /notice %}}
Etherpads have no user rights management, everyone can write and overwrite other texts (caution!). If user management is needed, better use [Nextcloud Text](https://github.com/nextcloud/text) (contact TUD cloudstore) or [CodiMD](https://md.inf.tu-dresden.de/)


## Element Matrix Services (EMS) offers Bridge for Microsoft Teams

To bringt together users from Element & MS Teams EMS offers a MS Teams Bridge, which you have to pay for:
[https://element.io/blog/ems-launches-bridging-for-microsoft-teams/](https://element.io/blog/ems-launches-bridging-for-microsoft-teams/) and [https://element.io/blog/microsoft-teams-and-slack-integration-using-matrix/](https://element.io/blog/ems-launches-bridging-for-microsoft-teams/).


## Custom widget

Any Internet pages can be integrated. For example [CodiMD](https://md.inf.tu-dresden.de/) to display LaTeX formulas.


