---
title: "Format messages"
date: 2020-07-15T18:05:37+02:00
draft: false
chapter: true
weight: 30
---

## Write and read messages

Messages can be sent with the **Enter key**. For a line break press Shift + Enter.

![Explanation of the symbols in the text input line](/images/01_Textformatting_en.png)

**files** (also images) can be sent up to a size of 10MB. For this purpose the paper clip must be selected. The sidebar with the document symbol shows the files within a room. Larger files can be shared via the [cloudstore of TU Dresden](https://cloudstore.zih.tu-dresden.de) and a share link.

Using text formatted in the markup language [**MarkDown**](https://de.wikipedia.org/wiki/Markdown), messages can also be formatted in Matrix Element. Here are some examples:

| result | to type |
|:------------------------------------------------------------------------------- |:-------------------------------------------------------------------------------------:|
| **Bold**                                                                        | ```**Bold**```                                                                        |
| *Italic*                                                                        | ```_Italic_```                                                                        |
| \| quote                                                                        | ```> quote```                                                                         |
| **Heading 1**                                                                   | ```# Heading 1```                                                                     |
| Heading 2                                                                       | ```## Heading 2```                                                                    |
| [Matrix Help](https://doc.matrix.tu-dresden.de/)                                | ```[Matrix Help](https://doc.matrix.tu-dresden.de/)```                                |
| ![TUD](https://tu-dresden.de/++theme++tud.theme.webcms2/img/tud-logo-white.svg) | ```![TUD](https://tu-dresden.de/++theme++tud.theme.webcms2/img/tud-logo-white.svg)``` |
| list entries                                                                    | ```* list entry```<br/>```* list entry```<br/>```* list entry```<br/>                 |
| numbered lists                                                                  | ```1. numbered list```<br/>```2. numbered list```<br/>```3. numbered list```<br/>     |

The current [MarkDown specification can be found here](https://spec.commonmark.org/current/).

The input of LaTeX formulas is currently not supported, but has already been requested: https://github.com/vector-im/element-web/issues/1945
Alternatively, an integration can be used to create a CodiMD (e.g. at https://md.inf.tu-dresden.de/), in which LaTeX can be used.

**Hashtags** can be used to make terms easier to find in the search.

**Smileys** can be reached with a starting colon ":"

![Opened Emoji menu](/images/14_Direktnachricht14.webp)

If there are more unread messages in a room than the screen can display, clicking on the icon to the right of the central content with a triangle pointing up and a dot pointing up will make you jump to the oldest unread message.

![Mark the jump to the last unread message button](/images/18_Sprung_hoch.webp)
Similarly, you can jump to the latest timestamp of a conversation by clicking on the triangle at the bottom of a circle on the right edge of the central content page.

![Marking of the button jumping to the newest message](/images/18_Sprung_nach_unten.webp)

A theme-based presentation (also called "threading") that is similarly good as [Zulip](https://en.wikipedia.org/wiki/Zulip) (by themes in each room/group/stream/channel) or in other programs by using a 3rd column does not exist with Matrix/Element, but is available as a wish: https://github.com/vector-im/element-web/issues/2349
