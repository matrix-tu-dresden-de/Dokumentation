---
menutitle: "Blog/News"
title: "Blog"
date: 2020-01-02T21:26:25+02:00
draft: false
weight: 200
---


***
#### 30.11.2021 - Exchange of experiences with Max-Planck-Society and further schools of higher education {#experience-exchange}

The efforts of TU Darmstadt and Karlsruhe Institute of Technology (KIT) in setting up a central Matrix instance are supported by TU Dresden with the exchange of experiences with our setup. Also, the Max-Planck-Society with its 83 institutes considers, after 3 years running Mattermost, to switch to Matrix. They invited TU Dresden as well to an exchange of experiences. Further attendees were representatives of the [TI-Messenger](https://www.gematik.de/anwendungen/ti-messenger/) of gematik and the [Bw-Messenger](https://messenger.bwi.de/) of Bundeswehr.


#### 11.10.2021 - Export room content easily {#export}

Since Element version 1.9.1 it is possible to export the room contents in a .html, .txt or .json file. Many thanks to [Jaiwanth Vemula from IIT Kharagpur University in India](https://element.io/blog/element-1-9-1-export-is-finally-here/)!

![Export room content](https://element.io/blog/content/images/size/w1000/2021/10/Screenshot-2021-10-11-at-10.21.21.png)

#### 08.10.2021 - Spaces {#spaces}

Spaces stands for the possibility to group rooms and also to give other people access to many rooms, e.g. to invite them to one Space instead of inviting them to many rooms.
This is ideal for students of one year, whose Space contains all rooms of all courses. Or for working groups, whose different subject rooms are bundled here and thus offer new team members quick access to all rooms.
Spaces replace the previous communities as room filters

[1] https://element.io/blog/spaces-blast-out-of-beta/
[2] https://element.io/blog/spaces-the-next-frontier/
[3] https://gnulinux.ch/element-spaces


![Add room to Space](https://element.io/blog/content/images/2021/09/spaces-add-existing-02-min.gif)
![Share a Space](https://element.io/blog/content/images/size/w1000/2021/09/Invite@2x.png)

#### 16.08.2021 - Voice messages in Matrix/Element {#sprachnachrichten}

Since Element version 1.8, [Voice messages](https://element.io/blog/introducing-voice-messages-and-so-much-more/) are easily recordable and sendable.

![Voice messages](https://element.io/blog/content/images/2021/08/output-1.gif)

#### 27.07.2021 - German healthcare receives Matrix Messenger

The German Ministry of Health announces the adoption of Matrix as the messaging standard for the German healthcare system starting in 2022. The [Gematik](https://fachportal.gematik.de/anwendungen/ti-messenger) cites the following primary reasons for this choice:
The Matrix open-source messenger protocol ensures:
- Interoperability - and thus cross-sector and cross-provider exchange.
- Integrity thanks to a high level of out-of-the-box security,
- End-to-End Encryption, and
- Innovation through continuous further development.

#### 13.06.2021 - TU Dresden has more than 20,000 Matrix users {#20000}

In the meantime, more than half of the TU Dresden members have already tried Matrix.

[![20.000 Matrix User @ TU Dresden](/images/blog/20210613_20000_Matrix_User.png)](https://doc.matrix.tu-dresden.de/Statistik/matrix-logins.html)


#### 11.05.2021 - Matrix Testimonials

Members of the TU Dresden express their assessment of Matrix. (We apologize that the testimonials are only in German.)

<img id="image-id" style="width: 1280px; max-width: 100%; margin-left:0;">
<script>
var cssSelector = "#image-id";
var imageFolderPath = "/images/statements";
var imageCount = 19;
var displayTime = 30000; //in ms
document.querySelector(cssSelector).src = imageFolderPath+"/"+Math.floor(Math.random() * imageCount)+".jpg";
setInterval(() => {
    document.querySelector(cssSelector).src = imageFolderPath+"/"+Math.floor(Math.random() * imageCount)+".jpg";
}, displayTime);
</script>

#### 28.04.2021 - Secure collaboration in education

TU Dresden appears on the [Element Blog](https://element.io/blog/universal-universities/) and an [Element Education Sector page](https://element.io/sectors/education) as a successful installation example and with the instance map.
ETH Zurich](https://matrix.org/using-matrix/case-studies/eth-zurich-adopts-matrix-for-physics-department) reports on how more and more teams are switching from Slack to Matrix.
And [Uni Innsbruck](https://element.io/case-studies/university-of-innsbruck) explains in detail their path to Matrix adoption.

#### 27.03.2021 - Relogin

Due to an update on the Matrix server, the locations for media files have changed. Clients that have been logged in since before 03/28/2021 will no longer see media. To resolve this issue, a one-time logout and re-login is required. To ensure that no previous encrypted messages become unreadable in the process, the [procedure described in the FAQ]({{< relref "faq/_index.md" >}}) must be followed urgently! Our big advantages from this: As of now, however, our matrix setup is a [MDAD](https://github.com/spantaleev/matrix-docker-ansible-deploy) with automatic configuration of synapse workers and a reduction in the risk of attack by cross-site scripting (XSS).

#### 02.03.2021 - Pull request for MDAD synapse worker successfully flagged

TU Dresden can be proud of this contribution to the Matrix development! Over the weekend, Pull Request (proposal for improved program code) with the number [456](https://github.com/spantaleev/matrix-docker-ansible-deploy/pull/456) was accepted within the Matrix Docker Ansible Deploy (MDAD) repository and incorporated into the master branch, which was initiated and significantly co-developed by the TU Dresden over the last 10 months.
The code adaptations, which have already made the Dresden Matrix service stable since April 2020 for meanwhile > 18,000 users through targeted load balancing on so-called *synapse workers*, were further developed collaboratively by several people and are now freely available to all MDAD users worldwide.
The TU Dresden has proven here once again that the promotion of free software is not only possible through the financial support of a group of developers or the direct commissioning for the development of new features ([example LibreOffice](https://osb-alliance.de/pressemitteilungen/osb-alliance-meldet-erneut-erfolgreiches-crowdfunding-von-libreoffice-verbesserungen) or [example PDF signatures with Okular](https://forums.puri.sm/t/okular-digital-signatures-and-tu-dresden/13808)). If there is hardly any money available, there is still the possibility to feed back own developments to the global community.
The exploitation of synapse-worker through pull request 456 enables other large institutions (e.g. the many universities that also use Matrix) to operate a stable, scalable instance.

#### 22.01.2021 - Post at *This Week in Matrix (TWIM)*

The release of the bilingual [Matrix documentation on GitHub](https://github.com/matrix-tu-dresden-de/Dokumentation) as well as the [Instance Map of German Universities](https://doc.matrix.tu-dresden.de/why/) led to an invitation to an [Interview for *This Week in Matrix (TWIM)*](https://matrix.org/blog/2021/01/22/this-week-in-matrix-2021-01-22#superb-documentation-from-tu-dresden-as-they-roll-out-their-deployment). Here Marvin Dropp and Christian Bruchatz presented the documentation as well as the interactive SVG of the instance map and reported about the Matrix developments at the TU Dresden.

[![TWIM-Interview 22.01.2021](/images/blog/04_TWIM-2021-01-22.png)](https://invidio.xamh.de/watch?v=UHJX2pmT2gk)

[![Matrix Doku auf GitHub](/images/blog/02_TUD-Matrix-Doc-Github-Repo.png)](https://github.com/matrix-tu-dresden-de/Dokumentation)

#### 22.01.2021 - Instance map for universities

Colleges and universities known to us with a Matrix service are now represented in a map that can be further developed by others [on GitHub](https://github.com/matrix-tu-dresden-de/Dokumentation/blob/main/static/images/federation_map.svg).
Networking with Matrix admins at other universities goes hand in hand with this and ensures an increasing exchange of experiences.
Being named on the map does not necessarily mean that the server there is also federating with others.

<object data="/images/federation_map.svg" type="image/svg+xml" style="width: 600px; max-width: 100%"></object>

#### 15.01.2021 - Matrix documentation receives overview graphic

An interactive SVG gives an overview of the functionality and appearance of Matrix/Element on the documentation home page. The download links for Element are also quickly accessible this way:

<object data="/images/matrix_interactive.svg" type="image/svg+xml" style="width: 1280px; max-width: 100%"></object>

#### 05.01.2021 - Extensive server monitoring

Prometheus und Grafana

#### 15.07.2020 - Riot becomes Element

The less suitable name *Riot* for the referent client is put aside and with Element the Matrix naming world of the company New Vector Ltd. enriches itself again in the mathematical milieu. Suitable also for a technical university.

[1] https://element.io/blog/welcome-to-element/
[2] https://element.io/previously-riot

#### 01.07.2020 -  More intensive further development thanks to CIO support

So far, various TUD offices have funded different student assistants from time to time to maintain and further develop the Matrix setup at TU Dresden. Since July, funding from the CIO is now also in place, giving the whole project a significant boost and giving new student administrators the opportunity to help TU Dresden improve its communication infrastructures! Many thanks to the CIO for this funding and Prof. Sander for his input in the CIO Advisory Board meeting on 27.4.2020.

#### 07.05.2020 - Cross-Signing

Prof. Jochen Plikat (Institute of Romance Studies) explains how securing the keys of encrypted chats in Matrix works, and what role the new "cross-signing" function plays in this context. [Direct to video](https://invidio.xamh.de/watch?v=VOxfa6dqXSk)

[![Cross-signing (Quersignierung) erklärt](/images/blog/keyserver.jpg)](https://jochen-plikat.com/2020/05/07/riot-cross-signing/)

#### 06.04.2020 - Introduction of synapse workers

We use [Matrix-Docker-Ansible-Deploy (MDAD)](https://github.com/spantaleev/matrix-docker-ansible-deploy), a mesh of Ansible roles for the various Matrix services in Docker containers with systemd control. In this framework, support for the experimental [synapse workers](https://github.com/matrix-org/synapse/blame/master/docs/workers.md) has not been implemented by anyone yet, there is a [feature request](https://github.com/spantaleev/matrix-docker-ansible-deploy/issues/221) for this from TU Dresden as of today. This integration (i.e. adaptation of the Ansible roles) has to be done, so that an optimal usage of the hardware (CPU cores) can be guaranteed and the TUD Matrix homeserver can be operated performantly in the long run. Many thanks to Marcel Partap for the work on a [Pull Request](https://github.com/spantaleev/matrix-docker-ansible-deploy/pull/456) and the parallel manual adjustments here at the TU Dresden, a development at the open heart so to speak...!

#### 16.03.2020 - Strong increase in demand due to Corona {#corona}

Start of nationwide homeschooling = home office for all with school-age children. Currently without dedicated funding, the decentralized Matrix admin team, especially with students, is committed to ensuring the demanded communication infrastructure due to the acute need. Special thanks go to Christoph Johannes Kleine and Marcel Partap! But also all around the Matrix Admin Team we see a professionalization, with a OTRS ticket queue, a central Matrix mail, and a public Support-Room.

Teachers start preparing for a digital summer semester and Prof. Alexander Lasch (Institute of German Studies) helps everyone to discover new tools, including the TUD Matrix Messenger. Others, like Dr. Eike Dohmen, help with a PDF guide to Matrix usage that circulates within the university.... Thanks also for all this support!

[![Digitale Lehre 1: MATRIX Web Messenger](/images/blog/20210316_Matrix_TUDresden.jpg)](https://invidio.xamh.de/watch?v=AtkA-sE-9uU)

#### 29.01.2020 - Global federation, firewall release for matrix.tu-dresden.de and restart of server monitoring {#firewall}

The TUD Matrix Messenger is now accessible worldwide and federated with many partner institutions. Previously, the new registration of [number of new users](https://doc.matrix.tu-dresden.de/Statistik/matrix-logins.html) started from 10.01.. This shows how Matrix is developing at TU Dresden.

[![TUD Matrix User](/images/blog/20200403_Matrix_TUD_User.png)](https://doc.matrix.tu-dresden.de/Statistik/matrix-logins.html)

#### 01.10.2019 - TU-internal pilot operation at matrix.tu-dresden.de begins {#stable}

After completion of the approximately one-year beta phase, pilot operation within the TU Dresden will now begin under the new domain [matrix.tu-dresden.de](https://matrix.tu-dresden.de), following consultation with the CIO.

[![TUD Matrix Web-Client](/images/blog/TUD_Element_Web.jpg)](https://matrix.tu-dresden.de)

#### 01.06.2019 - Importance of Matrix is perceived in many places

"The only app that meets all relevant criteria for an alternative to WhatsApp is Riot," writes Jun.-Prof. Jochen Plikat (Institute of Romance Studies) in his [blog post](https://jochen-plikat.com/2019/06/01/whatsapp-alternative-riot/). He goes on to cite the introduction of a Matrix-based chat system "[for all French state employees](https://www.golem.de/news/statt-whatsapp-frankreich-wandert-in-die-matrix-1902-139167.html)."


#### 15.04.2019 - CIO presentation on recommendations of internal digital communication {#cio-vortrag}

The [Team Initiation & Interaction (TII)](https://tu-dresden.de/tu-dresden/profil/exzellenz/exzellenzinitiative-2012-2019/zukunftskonzept-1/zse/archiv) advises the CIO Advisory Board of TU Dresden which free tools would improve the digital infrastructures for internal communication and collaboration and how scientists at TU Dresden could be helped the most. Matrix is presented as the central and most important tool. The support of numerous IT-representatives confirmed the chosen path. Due to a lack of financial resources, further development is not directly supported by the CIO, but tolerated under the self-organization of a decentralized admin team. From now on, this team will work under the auspices of the CIO of the School of Science, Prof. Dr. Oliver Sander, and under the coordination of the TII. For a short-term continuation of the work of the student assistants, we would like to thank the Chair of Software Technology and the [Team Initiation & Interaction](https://tu-dresden.de/tu-dresden/profil/exzellenz/exzellenzinitiative-2012-2019/zukunftskonzept-1/zse/archiv) for their financial support.

[![CIO-Präsentation](/images/blog/20190419_CIO-Vortrag.png)](https://doc.matrix.tu-dresden.de/images/blog/20190415_CIO-Meeting_KollaborativeTools.pdf)

#### 10/2018 - Matrix-Testserver goes online {#testserver}

After tests with [Mattermost](https://de.wikipedia.org/wiki/Mattermost), [Rocket.Chat](https://en.wikialpha.org/wiki/Rocket.chat) and [Zulip](https://en.wikipedia.org/wiki/Zulip), the [Team Initiation & Interaction (TII)](https://tu-dresden.de/tu-dresden/profil/exzellenz/exzellenzinitiative-2012-2019/zukunftskonzept-1/zse/archiv) launches the first Matrix homeserver at https://matrix.tii.tu-dresden.de and tests it with interdisciplinary communities from the TU Dresden and its surrounding cooperation partners. Many thanks to Joris Baum for the initial Synapse installation and to the [Hochschulgruppe Freie Software Freies Wissen](https://fsfw-dresden.de/), esp. to Marcel Partap and Christoph Johannes Kleine, for the intensive further development. Many thanks are also due to the [Center for Information Services and High Performance Computing (ZIH)](https://tu-dresden.de/zih/) as well as the [School of Science](https://tu-dresden.de/mn/der-bereich/leitung-und-verwaltung) for the financial support of the initial student assistants.

#### 06/2018 - Planning start{#start}

In the course of preparing for the expected digital, asynchronous collaboration in the Cluster of Excellence *DCM - Dresden Center for Materiomics*, the [Team Initiation & Interaction](https://tu-dresden.de/tu-dresden/profil/exzellenz/exzellenzinitiative-2012-2019/zukunftskonzept-1/zse/archiv) started to design the future internal communication of the cluster. A first presentation takes place in the CAB meeting of the Center for Information Services and High Performance Computing (ZIH) in August 2018 and sets the ground for the further support of the Matrix project by ZIH.
