---
title: "Nachrichten formatieren"
date: 2020-07-15T18:05:37+02:00
draft: false
chapter: true
weight: 30
---

## Nachrichten schreiben und lesen

Nachrichten können mit der **Enter-Taste** versendet werden. Für einen Zeilenumbruch drückt man Umschalt + Enter.

![Erläuterung der Symbole in der Texteingabezeile](/images/01_Textformatting_de.png)

**Dateien** (auch Bilder) lassen sich bis zu einer Größe von 10MB versenden. Dazu ist die Büroklammer auszuwählen. Die Seitenleiste mit dem Dokumentensymbol zeigt die Dateien innerhalb eines Raumes an. Größere Dateien können über die [cloudstore der TU Dresden](https://cloudstore.zih.tu-dresden.de) und einen Freigabelink geteilt werden.

Mittels Text, der in der Auszeichnungssprache [**MarkDown**](https://de.wikipedia.org/wiki/Markdown) formatiert ist, lassen sich auch in Matrix Element Nachrichten formatieren. Hier einige Beispiele:

| Ergebnis                                                                        | einzutippen                                                                                    |
|:------------------------------------------------------------------------------- |:----------------------------------------------------------------------------------------------:|
| **Fett**                                                                        | ```**Fett**```                                                                                 |
| *Kursiv*                                                                        | ```_Kursiv_```                                                                                 |
| \| Zitat                                                                        | ```> Zitat```                                                                                  |
| **Überschrift 1**                                                               | ```# Überschrift 1```                                                                          |
| Überschrift 2                                                                   | ```## Überschrift 2```                                                                         |
| [Matrix Hilfe](https://doc.matrix.tu-dresden.de/)                               | ```[Matrix Hilfe](https://doc.matrix.tu-dresden.de/)```                                        |
| ![TUD](https://tu-dresden.de/++theme++tud.theme.webcms2/img/tud-logo-white.svg) | ```![TUD](https://tu-dresden.de/++theme++tud.theme.webcms2/img/tud-logo-white.svg)```          |
| Listeneinträge                                                                  | ```* Listeneintrag```<br/>```* Listeneintrag```<br/>```* Listeneintrag```<br/>                 |
| Nummerierte Listen                                                              | ```1. Nummerierte Liste``` <br/>```2. Nummerierte Liste```<br/>```3. Nummerierte Liste```<br/> |

Die aktuelle [MarkDown-Spezifikation ist hier](https://spec.commonmark.org/current/) zu finden.

Das Eingeben von LaTeX-Formeln wird zur Zeit nicht unterstützt, wurde aber schon gefordert: https://github.com/vector-im/element-web/issues/1945
Alternativ kann mittels einer Integration ein CodiMD erstellt werden (z.B. unter https://md.inf.tu-dresden.de/), in welchem dann LaTeX verwendet werden kann.

**Hashtags** können benutzt werden um Begriffe leichter in der Suche auffindbar zu machen.

**Emojis** erreicht man mit einem beginnenden Doppelpunkt „:“ und dem Tippen von min. zwei weiteren Buchstaben. Wer gewünschte Emoji-Namen nicht auswendig kennt, kann mit Mausklick auf das Smiley-Zeichen rechts in der Eingabezeile durch viele Emojis scrollen.

![Aufeklapptes Emoji Menü](/images/14_Direktnachricht14.webp)

Wenn es mehr ungelesene Nachrichten in einem Raum gibt, als der Bildschirm anzeigen kann, lässt einen ein Klick auf das Symbol rechts vom zentralen Inhalt mit Dreieck nach oben und einem Punkt nach oben zur ältesten ungelesenen Nachricht springen.

![Makierung des Sprung zur letzten ungeleseen Nachrichtbuttons](/images/18_Sprung_hoch.webp)
Analog springt man zum neuesten Zeitstempel einer Unterhaltung durch Klick auf das Dreieck nach unten in einem Kreis am rechten Rand der zentralen Inhaltsseite.

![Makierung des zur neusten Nachricht-springen buttons](/images/18_Sprung_nach_unten.webp)

Eine Themenbasierte Darstellung (auch „Threading“ genannt), dass ähnlich gut ist wie bei [Zulip](https://en.wikipedia.org/wiki/Zulip) (durch Themen in jedem Raum/Gruppe/Stream/Channel) oder in anderen Programmen durch Nutzung einer 3. Spalte gibt es bei Matrix/Element nicht, ist aber als Wunsch vorhanden: https://github.com/vector-im/element-web/issues/2349
