---
menutitle: "FAQ"
title: "Frequently asked questions"
date: 2020-08-02T21:26:25+02:00
draft: false
weight: 200
---
This is a collection of frequently asked questions and their answers. Some of the answers are not yet written. In these cases please ask in the matrix room ```#matrix-support:tu-dresden.de```.

* [What is the difference between passphrase and recovery key?](#securityphrase-vs-securitykey)
* [Why is there no status bar at the bottom of the screen when hovering over hyperlinks in the Desktop-Client element? How can you trust them then?](#no-statusline)
* [How to tell people a room address with Element Desktop Client?](#desktop-share-room)
* [How do you tell people a room address with Element Web-Client?](#web-share-room)
* [Can I write LaTeX?](#latex)
* [Are there something like Threads (like in Mattermost/Slack) in Matrix?](#threads)
* [How do I change the passphrase for my key backup?](##change-securityphrase)
* [How do I reset the key backup if I have lost my passphrase AND my (saved and printed) recovery key?](#reset-securityphrase)
* [Why is there no room "TU Dresden"? Who is allowed to create it?](#no-tud-room)
* [How can I, as the administrator, delete many messages at once?](#delete-multiple-messages)
* [Sometimes I see a room marked in bold and click on it, but I don't have the time to edit the content and any consequences for me immediately. How can I mark the room as "unread" again?](#mark-room-as-unread)
* [What should I do if video or audio in a video conference does not work on a MacOS?](#apple-no-video)
* [How many people can be invited at ones into a room? Can I invite people by their E-Mail address?](#how-many-invites-can-i-do)
* [Can I modify access permissions for all rooms in my community, that only members of the community can enter?](#roompermissions-in-communities)
* [Can I manage multiple Matrix-Account on my Element Desktop Client?](#multiple-accounts-element)
***
#### What is the difference between passphrase and recovery key? {#securityphrase-vs-securitykey}
The password that can access the key backup is called the recovery key and is very long, starts with a capital E and should be saved or printed after setup. Since this password is hard to remember in everyday life (e.g. when you are on the road, want to have a look at Matrix, but only have access to other computers) you can think of a (easy to remember) passphrase from which the recovery key can be calculated (in the browser/client) before trying to "open" the key backup.

***
#### Why is there no status bar at the bottom of the screen when hovering over hyperlinks in the Desktop-Client element? How can you trust them then? {#no-statusline}
In fact, the status bar is a popular test of the seriousness of hyperlinks you are trying to click on. In the Desktop Client element this is not possible, similar to the mobile clients. Here you can only right-click on the link and check the presented target page for seriousness.

***
#### How to tell people a room address with Element Desktop Client? {#desktop-share-room}
With the matrix.to link, which you can see under the i for the room properties and another click on "Share room".

***
#### How do you tell people a room address with Element Web-Client? {#web-share-room}
With the matrix.to link, which you can see under the i for the room properties and a further click on "Part room" and an exchange of the front matrix.to with matrix.tu-dresden.de

***
#### Can I write LaTeX? {#latex}
Yes, but it is an experimental feature right now. It will be available for everybody in a few weeks: https://github.com/vector-im/element-web/issues/1945

***
#### Are there something like Threads (like in Mattermost/Slack) in Matrix? {#threads}
No, threads like in Mattermost or Slack are currently not existing in Matrix. The developers of Element are aware of this topic and planed it for future release. To get more information, follow their roadmap: https://github.com/vector-im/roadmap/projects/1

***
#### How do I change the passphrase for my key backup? {##change-securityphrase}
?
***
#### How do I reset the key backup if I have lost my passphrase AND my (saved and printed) recovery key? {#reset-securityphrase}
?
***
#### Why is there no room "TU Dresden"? Who is allowed to create it? {#no-tud-room}
All persons creating a room are administrative persons and are responsible for the room. Matrix is not yet designed for the exchange of thousands of members at the university. Should a central room be needed one day, its establishment and maintenance would certainly be the responsibility of the Rectorate and the Department of "Strategy & Communication".

***
#### How can I, as the administrator, delete many messages at once? {#delete-multiple-messages}
?
***
#### Sometimes I see a room marked in bold and click on it, but I don't have the time to edit the content and any consequences for me immediately. How can I mark the room as "unread" again? {#mark-room-as-unread}
Unfortunately this is not possible in Element. As a workaround, you can mark the room as a favorite and notice yourself that your own favorites should be looked at again.

***
#### What should I do if video or audio in a video conference does not work on a MacOS? {#apple-no-video}
Often Element does not have the rights to access the webcam and microphone. These can be assigned in the system settings under Security and Privacy.

***
#### How many people can be invited at ones into a room? Can I invite people by their E-Mail address? {#how-many-invites-can-i-do}
Mass invite by E-Mail is currently not supported in Element. If you want to mass invite, please send an request via the servicedesk, so we can assist. You can invite 100 people by their ZIH username yourself.  

***
#### Can I modify access permissions for all rooms in my community, that only members of the community can enter? {#roompermissions-in-communities}
No, this is not possible. Rooms can be part of multiple communities. Therefore the access permission will be set on room based level.


***
#### Can I manage multiple Matrix-Account on my Element Desktop Client? {#multiple-accounts-element}
With the Element Desktop client, you can only manage one Matrix-Account right now. But it is possible to start several Element-windows with different Matrix-Accounts, also within your Autostart-settings of your computer. Therefore, you need to change (or create additional) execution commands to open a specific profile:

``` 
element-desktop --profile PROFILE_NAME
``` 
So you can place several Element-Starters in your Autorstart, with different profile names, e.g. --profile TUD or --profile Private. Unfortunately, both opened windows will appear with the same Icon in the Indicator-Applet. But therefore, a solution will upcome soon, for sure...

Furthermore, there are other Matrix-Clients, that can handle more Matrix-Accounts per se, e.g. [weechat](https://matrix.org/docs/projects/client/weechat-matrix), [Spectral](https://matrix.org/docs/projects/client/spectral), [Quaternion](https://matrix.org/docs/projects/client/quaternion), or [Mirage](https://matrix.org/docs/projects/client/mirage).
