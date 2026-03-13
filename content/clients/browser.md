---
title: "Element Web (Browser)"
date: 2020-07-15T16:46:07+02:00
draft: false
chapter: true
weight: 5
---

# Element Web

Am einfachsten kann Matrix durch die vorkonfigurierte Element-Web-Anwendung unter [matrix.tu-dresden.de](https://matrix.tu-dresden.de) genutzt werden. Dadurch entfällt beispielsweise die Eingabe der Homeserver-URL beim Login und bestimmte Features sind aktiviert beziehungsweise deaktiviert.

![Startseite von Element Webclient mit Anmeldebutton](/images/01_Welcome_de.png)

Um Matrix zu nutzen ist keine Registrierung notwendig. Der Dienst kann sofort durch das Klicken auf „Anmelden“ auf der Startseite [matrix.tu-dresden.de](https://matrix.tu-dresden.de) genutzt werden.

![Loginfenster mit Aufforderung ZIH Login und Passwort einzugeben](/images/02_Login1_de.png)

Das Dropdown-Menü „Anmelden mit:“ sollte auf „Benutzername“ belassen werden. Dann sind folgende Eingaben zu tätigen:

**Benutzername: ZIH-Login**  (nur der ZIH-Login, keine E-Mail-Adresse!)

**Passwort: ZIH-Passwort**

Ein alternativer Login, bspw. über die E-Mail-Adresse ist **NICHT** beim ersten, initialen, Anmelden möglich, erst ab dem zweiten Einloggen.

Es folgt nach dem Erstlogin auch keine E-Mail / Bestätigungsmail.

Analog zu E-Mail-Adressen ergeben sich damit Matrix-Adressen folgender Struktur:

@ZIH-Login:tu-dresden.de

{{% notice warning %}}
Sollten Sie anstatt mit der Element-Web-App sofort mit einem [Matrix Client]({{< relref "../clients" >}}) starten wollen, ist es wichtig den Heimserver `matrix.tu-dresden.de` der TU Dresden einzustellen (siehe [Erste Schritte]({{< relref "../first-steps" >}})).
{{% /notice %}}

## Browsereinstellungen

### Browserwahl

Empfehlenswert sind die Browser [Firefox](https://www.mozilla.org/de/firefox/new/), [Chromium](https://www.chromium.org/getting-involved/download-chromium), neuere Versionen von Microsoft Edge (basierend auf Chromium). Ältere oder ungeeignete Browser zeigen unter Umständen nur eine weiße Seite an.

### NoScript

Sollten Sie Browser-Plugins (z.B. Skript-Blocker) nutzen, um sich vor [Tracking](https://tu-dresden.de/tu-dresden/newsportal/news/datenschutz-beim-website-tracking) und Schadsoftware im Browser zu schützen, beispielsweise mit dem Addon [NoScript](https://addons.mozilla.org/de/firefox/addon/noscript/). Hier sind folgende Einstellungen durchzuführen (für den Integrationsmanager, z.B. Jitsi/Etherpad)

![Einstellungen des Browserplugins NoScript mit tu-dresden.de und vector.im als vertrauenswürdige Skriptquellen ausgewählt](/images/10_Sicherheit2_de.png)

### Cookies

Erlauben Sie auch Cookies von

- tu-dresden.de
- vector.im (für den Integrationsmanager)
