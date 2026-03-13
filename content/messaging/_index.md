---
title: "Nachrichten"
date: 2020-07-15T18:10:07+02:00
draft: false
chapter: true
weight: 30
---

## Personen finden und direkte Nachrichten versenden

Um einzelne Personen anzuschreiben und einen privaten 1:1 Chat zu erzeugen, klickt man zunächst auf das + in der Kategorie „Direkte Nachrichten“:

![Klick au den Chat starten Button](/images/01_Start-Chat_de.png)

Nun kann in das Suchfeld die Matrix-Adresse (oder die E-Mail-Adresse) der Person eingeben werden, die man erreichen möchte. Nach dem letzten eingegebenen Zeichen sollten Sie bis zu fünf Sekunden warten, bis die Sucherergebnisse vollständig angezeigt werden. Beachten Sie auch, auf welchem Server Ihre gesuchte Person angezeit wird.

Personen, die schon einen Account in Matrix haben sind auch durch ihren Anzeigenamen (meist „Vorname Nachname“) auffindbar. Personen, die noch nicht eingeloggt waren, sind ausschließlich über ihre E-Mail-Adresse oder ihren ZIH-Login auffindbar. Der Link-Button „Show More“ lässt weitere Sucherergebnisse erscheinen.

Personen, die schon einen Account in Matrix haben sind auch durch ihren Anzeigenamen (meist „Vorname Nachname“) auffindbar. Bitte nach jedem letzten eingegebenen Zeichen 5 Sekunden warten, bis die Suchergebnisse angezeigt werden. Personen, die noch nicht eingeloggt waren, sind ausschließlich über ihre E-Mail-Adresse oder ihren ZIH-Login auffindbar. Der Link-Button „Show More“ lässt weitere Suchergebnisse erscheinen. Beachten Sie auch, auf welchem Server Ihre gesuchte Person angezeigt wird.

{{% notice note %}}
Ein Einfügen von Matrix-Adressen (zum Beispiel via `strg+v`) reicht nicht aus, um Personen zu finden! Am besten geben Sie die Zeichen der Matrix-Adresse per Hand ein (Zeichen für Zeichen). Bis alle Suchergebnisse vollständig angezeigt werden, kann es bis zu fünf Sekunden dauern.
{{% /notice %}}

Wenn Sie eine Person nicht finden können, fragen Sie nach deren Benutzernamen oder teilen Sie ihren Benutzernamen (`@<ZIH-Login>:tu-dresden.de`) oder https://matrix.to/#/@ZIH-Login:tu-dresden.de, damit die angesprochene Person Sie innerhalb von Matrix kontaktieren kann. Eine Einladungs-E-Mail wird durch nicht Matrix versendet.

![Ergebnis zugefügt zu den Personen, die in den Chat eingeladen werden](/images/99_Find-Neo_de.gif)

Für das massenhafte Einladen von Personen (bis zu 100 auf einmal, dann wiederholbar) sind die Matrix-Namen notwendig, die in der Form `@<ZIH-Login>:tu-dresden.de` vorliegen sollten. Diese bspw. in einem Texteditor Zeile für Zeile sammeln und dann mittels Zwischenablage (Kopieren & Einfügen) in das Suchfeld in Matrix/Element einfügen.

Beachten Sie, dass Matrix-Accounts von ZIH-Funktionslogins möglicherweise nicht geprüft werden. Aufgrund der Neuheit des Mediums für Viele sowie der fehlenden Multi-Account-Funktionalität vom Matrix-Client Element, werden TU Dresden Mitarbeitende womöglich eher ihren persönlichen ZIH-Login nutzen.

Im Suchergebnis klickt man auf die Zielperson und anschließend auf "Los":

![Ein Suchergebnis auf eingegebenen Suchanfrage](/images/04_Found-and-Go_de.png)

Es öffnet sich das Gespräch, welches nach Annahme der Einladung durch die verbundene Person [Ende-zu-Ende-verschlüsselt]({{< relref "encryption" >}}) (inzwischen Standard) beginnen kann. Die Verbindung zum Server an der TU Dresden ist natürlich auch transport-verschlüsselt. Sollten Sie aus einem speziellen Grund explizit keine Ende-zu-Ende-Verschlüsselung wünschen, wäre ein unverschlüsselter [Raum zu erzeugen]({{< relref "rooms/create.md" >}}) und die Gesprächspartner:in in diesen einzuladen.

### Einladen von Personengruppen

Für das Einladen von mehreren Personen (bis zu 25 auf einmal, dann wiederholbar) müssen die Matrix-Adressen in der Form `@<tu_login>:matrix.tu-berlin.de` vorliegen. Diese können Sie beispielsweise in einem Texteditor Zeile für Zeile sammeln und dann mittels Zwischenablage (Kopieren & Einfügen) in das Suchfeld in Matrix/Element einfügen.

### Raum als Zwischenablage verwenden

Es ist möglich einen Raum mit sich selbst zu erstellen. In diesem Raum ist man also der einzige Teilnehmer. Dieser Raum kann dann als Zwischenablage / Notizbuch sowie für Tests benutzt werden, zum Beispiel um zu prüfen ob Formatierungen (zum Beispiel von Latex) und Hyperlinks korrekt funktionieren.

### Weiteres
* [Nachrichten formatieren]({{< relref "formatting.md" >}})
* [Nachrichten suchen]({{< relref "search.md" >}})
