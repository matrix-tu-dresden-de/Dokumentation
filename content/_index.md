---
title: "Matrix an der TU Dresden"
date: 2020-08-02T21:26:25+02:00
chapter: false
draft: false
---

## Matrix an der TU Dresden
Matrix ist ein freies und offenes, sicheres, dezentralisiertes Protokoll für Echtzeit-Kommunikation, das auch unter dem Namen eines seiner nutzenden Programme, Element, bekannt ist.

<object data="/images/matrix_interactive.svg" type="image/svg+xml" style="width: 1280px; max-width: 100%"></object>

Zur Zusammenarbeit in Teams stieg in den letzten Jahren der Bedarf an unterstützenden digitalen Werkzeugen. Ein zentrales Werkzeug ist dabei ein Team-Chat. Ein Chat bezeichnet, laut Wikipedia, „die elektronische Kommunikation mittels geschriebenem Text in Echtzeit, meist über das Internet“ ([Quelle](https://de.wikipedia.org/wiki/Chat)). Mit einem Messenger (die Software zum Chatten) können sich Teammitglieder gegenseitig auf aktuelle Informationen aufmerksam machen und insbesondere Verknüpfungen (*Hyperlinks* / *Links*) zur weitergehenden Zusammenarbeit teilen (beispielsweise zur Terminfindung, zum kollaborativen Schreiben, zum Planen von Events, zum Bearbeiten von Daten, Code, Mindmaps oder Prozessen). Viele Teams an der TU Dresden haben sich aufgrund des bisher fehlenden zentralen Angebots eigene Lösungen gesucht, die zum Teil datenschutzbedenklich sind oder nicht mit anderen Systemen verknüpfbar sind.

Zur Deckung des Bedarfes an Echtzeitkommunikation wurde daher Ende 2018, nach vergleichender Analyse mehrerer potentieller Lösungsoptionen, innerhalb der TU Dresden das offene Kommunikationsprotokoll Matrix in einem Pilotbetrieb eingeführt und im April 2019 im CIO präsentiert. Im Herbst 2019 wurde der Pilotbetrieb in den Regelbetrieb überführt. U.a. in der [digitalen](https://invidio.xamh.de/AtkA-sE-9uU) [Lehre](https://invidio.xamh.de/jEvKdFTKSxU) (Videos von Prof. Lasch) findet Matrix als Ergänzung zu [OPAL](https://bildungsportal.sachsen.de/opal) Anwendung.

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

## Themen der Dokumentation

* [Warum Matrix und kein anderes Chat-System?]({{< relref "why/_index.md" >}})
* [Wie kann Matrix genutzt werden? (Anmeldung und erste Schritte)]({{< relref "first-steps/_index.md" >}})
* [Empfehlungen zu weiteren wichtigen Einstellungen nach dem Erstlogin]({{< relref "settings/_index.md" >}})
* [Matrix-Clients installieren und einrichten]({{< relref "clients/_index.md" >}})
    * [Element Web]({{< relref "clients/browser/_index.md" >}})
    * [Element Desktop]({{< relref "clients/desktop/_index.md" >}})
    * [Element Android]({{< relref "clients/android/_index.md" >}})
    * [Element iOS]({{< relref "clients/ios/_index.md" >}})
    * [Element-Installation unter Linux]({{< relref "clients/install_linux/_index.md" >}})
    * [Weitere Clients]({{< relref "clients/more_clients/_index.md" >}})
* [Personen finden und direkte Nachrichten versenden]({{< relref "messaging/_index.md" >}})
    * [Nachrichten formatieren]({{< relref "messaging/formatting/_index.md" >}})
    * [Nachrichten suchen]({{< relref "messaging/search/_index.md" >}})
* [Räume erstellen und Verantwortung übernehmen]({{< relref "rooms/_index.md" >}})
    * [Räume erstellen]({{< relref "rooms/create/_index.md" >}})
    * [Räume finden]({{< relref "rooms/find/_index.md" >}})
    * [Räume löschen und aus Räumen austreten]({{< relref "rooms/delete/_index.md" >}})
    * [Räume teilen und publik machen]({{< relref "rooms/sharing/_index.md" >}})
* [Benachrichtigungen feiner einstellen]({{< relref "notifications/_index.md" >}})
* [Communities als Raum-Filter einsetzen]({{< relref "communities/_index.md" >}})
* [Spaces zur Raumverwaltung einsetzen]({{< relref "spaces/_index.md" >}})
* [Ende-zu-Ende-Verschlüsselung nutzen]({{< relref "encryption/_index.md" >}})
* [Integrations, Bridges, Bots nutzen (u.a. Jitsi)]({{< relref "integrations/_index.md" >}})
* [Häufige Fragen (FAQ)]({{< relref "faq/_index.md" >}})
* [Weiterentwicklung von Matrix]({{< relref "development/_index.md" >}})
* [Blog/News]({{< relref "blog/_index.md" >}})
* [Datenschutzerklärung]({{< relref "privacy/_index.md" >}})
* [Impressum]({{< relref "imprint/_index.md" >}})
* [Nutzungsbedingungen]({{< relref "termsofuse/_index.md" >}})
* [Barrierefreiheitserklärung]({{< relref "accessibility/_index.md" >}})

### Fragen / Kontakt

Allgemeine Fragen richten Sie bitte an den [Service Desk](https://tu-dresden.de/zih/dienste/service-desk) der TU Dresden.

Probleme und deren Lösungen können darüber hinaus im [Matrix-Support-Raum](https://matrix.tu-dresden.de/#/room/#matrix-support:tu-dresden.de) diskutiert werden, sodass andere Nutzende durch den transparenten Austausch lernen können.

{{% notice tip %}}
Man kann bei manchen Anomalien probieren den Cache (Zwischenspeicher) zu leeren und alles neu zu laden: Einstellungen > Hilfe & Über > Cache löschen und neu laden
{{% /notice %}}

{{% notice note %}}
Aktuelle Wartungen werden in dem Matrixraum [#Matrix-Betriebsstatus:tu-dresden.de](https://matrix.tu-dresden.de/#/room/#Matrix-Betriebsstatus:tu-dresden.de) angekündigt.
{{% /notice %}}
