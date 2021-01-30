---
title: "Share rooms"
date: 2020-07-02T21:23:14+02:00
chapter: true
draft: false
weight: 40
---
# Share rooms and make them public
 {{% notice warning %}}
The share icon in the upper right corner of each room also provides a link, a QR code and various social networks. The link, however, leads to https://matrix.to/ from where you can access the room via an Element web app from https://element.io. In order to share a room within TU Dresden please use the methode explained in this artice.
 {{% /notice %}}
Every room has a so-called room-address, which can be found in the room settings under the sub-menu Advanced. A room address looks like this:

!aen6iekahv8Pi0zohf:tu-dresden.de

Because this cryptic address can not be read easily by humans, custom room addresses can be assigned. This is only necessary for rooms, which you want to make public and reference in other places.

Room addresses can either be globally published addresses (findable by users in other servers - useful for topics beyond the TU Dresden) or local addresses, which is only valid within the matrix home server at the TU Dresden.

{{% notice note %}}    
To publish a global address, you have to create a local address first. **It is necessary to create a local address in both cases!**
{{% /notice %}}  

For the more common case of the desired local address, click on "Show more" under Local Addresses in the room settings under the General tab:

![Room settings with the show more selected](/images/01_Sharing_en.png)

Afterwards a recognizable name of this room link can be assigned in the "Room alias" line (no spaces are allowed!):

![Room settings with the local addresses selected](/images/02_Sharing_en.png)

You can also assign different addresses. If the room address should be published in the room directory of the matrix home server of the TU Dresden, this can be done by the following. 

![room settings with the public room address selected](/images/03_Sharing_en.png)

The room address then has the following structure

#Room-address-name:tu-dresden.de

**Suggestion Nr. 1 for sharing a room address:**

When you want to share a room within matrix, you can use the internal link feature by typing (the first characters of) the local address
```
#room_address:tu-dresden.de
```
into the chat line. If you are a member of that room, you can confirm the auto-completion with a mouse click. This is a special link for a usage within matrix, which will open directly in the client of the receiver (with a mouse click).


**Suggestion Nr. 2 for sharing a room address:**

The share icon at the top right of each room also offers a matrix.to-link, as well as a QR code and various social networks. The matrix.to-link leads to a page where you can select how the link should be opened. For example, the installed client Element Desktop can be used, or it can be selected via which home server the room is to be entered. 

![share icon marked in the chat view of the room](/images/04_Sharing-Button_en.png)

```
https://matrix.to/#/#Room-address-name:tu-dresden.de?via=tu-dresden.de
```

**Suggestion Nr. 3 for sharing a room address:**

Furthermore, you also can create a hyperlink to the room, which you have to construct in this way:

https://matrix.tu-dresden.de/#/room/#roomaddress:tu-dresden.de

resulting in an internet address (URL) which can be easily distributed to the public or target group. BUT, **this link opens only an Element Web in the browser** of the people, not in an installed Element Desktop. More universal (espc. for the large group of people with Element Desktop), and more advised by the Matrix-Admin-Team, is the above mentioned method with the matrix.to-Link.
