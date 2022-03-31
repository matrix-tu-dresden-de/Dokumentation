---
menutitle: "FAQ"
title: "Frequently asked questions"
date: 2020-08-02T21:26:25+02:00
draft: false
weight: 200
---
This is a collection of frequently asked questions and their answers. Some of the answers are not yet written. In these cases please ask in the matrix room ```#matrix-support:tu-dresden.de```.

* [Messages not readable](#message-not-readable)
* [What is the difference between passphrase and recovery key?](#securityphrase-vs-securitykey)
* [Why is there no status bar at the bottom of the screen when hovering over hyperlinks in the Desktop-Client element? How can you trust them then?](#no-statusline)
* [How to tell people a room address with Element Desktop Client?](#desktop-share-room)
* [How do you tell people a room address with Element Web-Client?](#web-share-room)
* [Can I write LaTeX?](#latex)
* [Are there something like Threads (like in Mattermost/Slack) in Matrix?](#threads)
* [I do not have a security key (recovery key)](#no-security-key)
* [How do I change the passphrase for my key backup?](#change-securityphrase)
* [How do I reset the secure backup if I have lost my security phrase AND my (saved and printed) security key?](#reset-securityphrase)
* [Why is there no room "TU Dresden"? Who is allowed to create it?](#no-tud-room)
* [How can I, as the administrator, delete many messages at once?](#delete-multiple-messages)
* [Sometimes I see a room marked in bold and click on it, but I don't have the time to edit the content and any consequences for me immediately. How can I mark the room as "unread" again?](#mark-room-as-unread)
* [What should I do if video or audio in a video conference does not work on a MacOS?](#apple-no-video)
* [How many people can be invited at ones into a room? Can I invite people by their E-Mail address?](#how-many-invites-can-i-do)
* [Can I modify access permissions for all rooms in my community, that only members of the community can enter?](#roompermissions-in-communities)
* [Can I manage multiple Matrix-Account on my Element Desktop Client?](#multiple-accounts-element)
* [I can no longer see profile/room pictures or other pictures.](#relogin)

#### Messages not readable {#message-not-readable}
  * At least one verified session must be open at all times, the easiest way to do this is to set up the Desktop Client or Element on a smartphone. These programs can be closed and restarted without having to log in again. Otherwise, a verified Matrix session can be created in a private web browser window by logging into Matrix there and verifying this session from an existing one. This window can be closed after about five minutes. The keys are transferred to the other Matrix clients by the verification process. This creates a ghost session which is then always open. Then all other clients can be logged out. Otherwise messages which are received in the period without open matrix session cannot be read later. This is to be solved in the future by means of the function dehydrated devices.
  * Has the [Secure Backup]({{< relref "settings/#secure-backup" >}}) been set up properly?
  * Messages remain unreadable when matrix sessions are created and then the web browser window is simply closed without logging out. Solution: only possible for new messages: read this documentation.

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
With the matrix.to link, which you can see under the i for the room properties and a further click on "Part room" and an exchange of the front matrix.to/#/ with matrix.tu-dresden.de/#/room/

***
#### Can I write LaTeX? {#latex}
Yes, but it is an experimental feature right now. It will be available for everybody in a few weeks: https://github.com/vector-im/element-web/issues/1945

***
#### Are there something like Threads (like in Mattermost/Slack) in Matrix? {#threads}
Threads like in Mattermost or Slack are currently available as lab feature in Matrix and will be stable within the next weeks. To get more information, follow their roadmap: https://github.com/vector-im/roadmap/projects/1

***
#### I do not have a security key (recovery key) {#no-security-key}
To do this, please check whether this has been set up at all. See [Secure backup]({{< relref "settings/#secure-backup" >}})

***
#### How do I change the passphrase for my key backup? {#change-securityphrase}
  * export the room keys for all matrix sessions except for one, which is still accessible, `Settings` -> `Security & Privacy` -> `Encryption`/`Cryptography`, here it is best to provide the matrix login password. Finally, log out by clicking on the user name in the upper left corner and log out. If you are asked whether you want the encrypted messages, click on 'I don't want my encrypted messages', because these keys have already been exported.
  * Under `Settings`-> `Security & Privacy` -> `Secure Backup` press first `Delete Backup`, afterwards the button `Reset` and may a clearing of the cache under `Settings`-> `Help & About` is necessary, as well a logging off and logging on again. If all this does not work, continue in the next point. The action was successful, if only the green 'Setup' button is displayed.
  * For all previously exported key backups, perform the manual import path
  * Set up a new security backup. See [Secure backup]({{< relref "settings/#secure-backup" >}})

***
#### How do I reset the secure backup if I have lost my security phrase AND my (saved and printed) security key? {#reset-securityphrase}
Please execute the following:
  1. Export E2EE room keys manually in on Matrix session (=client/device/browser), where you can still read former encrypted conversation. Therefore, click on "Export E2EE room keys" under unter `Settings`-> `Security & Privacy` -> `Cryptography`. If you do not have any access to any Matrix session where you can read the former enrypted conversation, you have to skip this step.
  2. In the one Matrix session, where you manually exported your E2EE room keys, sign off all further devices in the following way: Tick all checkboxes for other sessions/devices/clients in `Settings`-> `Security & Privacy` -> `Where you're signed in` and afterwards click on the red "Sign out x selected devices" below the list. The entry at the top of the list under the subheadline "This device" should not be deleted.
  3. Maybe log out and log in again by ignoring all messages regarding the secure backup. Unfortuenately, you seem to not have the security key any more.
  4. Have a look in the `Settings`-> `Security & Privacy` -> `Secure Backup` if there is any green button `Set up Secure Backup`. If there are red buttons, start with clicking on `Delete backup`, continue with clicking on `Reset`. Maybe you should "Clear the cache and reload" under `Settings`-> `Help & About` and sign off and on again.
  5. Continue with clicking in `Settings`-> `Security & Privacy` -> `Cross-signing` on the red button `Reset`. This step was successful, if under the subheadlines `Secure Backup` and `Cross-signing` you only find green buttons for setting up. But do not click them right now in this step.
  6. Import your saved E2EE room keys from step 1 manually by using the button "Import E2EE room keys" in `Settings`-> `Security & Privacy` -> `Cryptography`.
  7. Now set up your new [Secure Backup]({{< relref "en/settings/#secure-backup" >}}) and the Cross-Signing with the two green buttons. Print the Security Key several times and deposit it securely (At only one place you have the risk of loss e.g. via a fire).

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

***
#### I can no longer see profile/room pictures or other pictures. {#relogin}
Due to an update on the Matrix server (28.03.2021), clients that have been logged in since then can no longer find media files. To solve this problem, it is necessary to log off and log on again. **Attention: So that you do not loose any of your messages you should follow the procedure below.** If multiple clients are affected, the procedure should be performed one after each other and not in parallel.

<ul type="1">
  <li>Make sure you have fulfilled at least one of the following prerequisites:</li>
  <ol type="a">
    <li>... an additional verified session (e.g. with the smartphone) is active and usable</li>
    <li>... the <a href="{{< relref "settings/#secure-backup" >}} ">Secure Backup</a> is set up and the security phrase or the security key are present</li>
    <li>... you have exportet your room keys</li>
  </ol>
  <li>Log off and log on again within the client and use as Matrix <strong>homeserver</strong>: "<strong>tu-dresden.de</strong>"</li>
  <li>Restore your messages:</li>
  <ol type="a">
    <li>... Verify the new session in the additional active session to start the key exchange between these sessions</li>
    <li>... Connect to the Secure Backup to get your message keys back</li>
    <li>... Import the room keys and set up the <a href="{{< relref "settings/#secure-backup" >}} ">Secure Backup</a></li>
  </ol>

**Annotations:**
* Losing the room keys will result in the loss of your messages, as they can only be read by you and your communication participants. No admin can help with that.
* Because of the new session, a red warning sign is subsequently displayed for all your previous messages. This is not an error, but just a little too dramatic information setting (further information can be found here: [external link](https://github.com/vector-im/element-web/issues/13701))
* If you only use Matrix on one device and you do not have access to your security phrase or security key you have to follow route c) to not loose your encrypted messages.


#### Everywhere I only see „missing translation: en“ {#missing-translations}

This phenomena is usually correlated with a not-ready update of the Matrix client. Reload the cache: Find the category „Help and About“ in your Element settings and scroll down: "Reload Cache" should solve this display problem.

#### Is our server on your federation blacklist? {#blacklist}

Currently we have no server on our federation blacklist. This cannot be the reason for your federation problem.

#### I do not see any message of a specific person in a room {#blocked-user}

A common reason for this is that you blocked that person by accident. You do not see any message of the person even if you hear that this person posted them. Open your Security settings in Element and scroll down. Please check in the category "Blocked user" if you find the person that does not belong there... Remove it!
