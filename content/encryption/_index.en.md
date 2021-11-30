---
title: "Encryption"
date: 2020-07-03T13:20:58+02:00
draft: false
chapter: true
weight: 60
---

# Use of end-to-end encryption

1:1 calls are now encrypted end-to-end by default. Therefore, a configured key backup as well as a verification of all self used client devices is recommended ([Important settings]({{< ref "settings" >}}))

The decision whether a created room should be encrypted in this way must be well thought out and cannot be undone. If the room is large or public, checking all keys of all interlocutors could take a lot of time. But this manual check can be done later on occasion and end-to-end encrypted conversations can be started directly with blind trust for the time being.

![Create new room with activated encryption](/images/01_Create-Room-wE2E_en.png)

If you want end-to-end encryption (E2EE) to interlocutor:inside in an unencrypted room, you can achieve this by clicking on the settings of the desired room. (or in the room via "Room info" > "Room settings" in the upper right corner):

![Menu to get to the room settings](/images/02_Roomsettings_en.png)

To do this, move the Encrypted slider on the Security & Privacy tab:

![Enable encryption in the room settings](/images/03_Roome2e_en.png)

This can be confirmed with OK. From now on the messages can only be read by those involved in the conversation. If you have not set up a key protection in the settings before, you should do this now (see [Important settings]({{< ref "settings" >}})) to be able to read earlier and in absence received messages.

Now the encrypted exchange can begin. If you want to verify the correctness of the keys and to document this trustworthiness digitally, you first have to unfold the sidebar by clicking on the person symbol in the upper right corner:

![open the list of persons in the room](/images/04_RoomPeople_en.png)

The contact person can now be clicked on in the opening bar of the participants in the conversation:

![room with note that not all participants are verified](/images/05_People-Unverified_en.png)

The bar now shows the conversation person in detail. Here a key verification can be initiated by clicking on "Verify". By clicking on "Start Verification" the other side is notified and after confirmation (see next picture) the "Verification by Emojis" can start.

![Menu to the person to verify selected with the verify button](/images/06_E2EE_Verify_en.png)

![Menu to start the verification](/images/07_E2EE_Accept_en.png)

This verification should be done with the contact person by comparison (e.g. verbally via telephone, in the same room or other medium). Since this is not always easy, the trust can also be expressed first of all (otherwise you will be asked again and again to carry out the verification) and carried out on occasion (e.g. at the next meeting).

A detailed description of the topic can be found in this [video by Prof. Plikat](https://invidious.ggc-project.de/VOxfa6dqXSk) and [in this Matrix blog article](https://blog.riot.im/e2e-encryption-by-default-cross-signing-is-here).

The adjustment itself is done via emoji images or QR codes, which can look different depending on the device and icon pack. Also the translation of all interface elements into German is not 100% available.

![Emoji comparison to verify the key exchange](/images/16_E2EE_en.png)

This is done analogously in rooms with several participants, each one individually. 

![verification process was successful](/images/08_Verified_en.png)

In the respective room rows the following symbols indicate the status of the encryption and the corresponding verification:

![symbol for at least one non-verified person](/images/gray.png)

At least one person in the room has not yet been verified.

![symbol for a verified person who has opened unverified sessions](/images/unverified.png)

There is at least one person in the room who has already been verified, but who in turn has opened further unverified sessions. 

![symbol for all persons in the room are verified](/images/green.png)

All persons in the room were verified.

Further example, how you can realise the encryption state of a room by checking the relevant icon next to the room icon in the room information panel at the top right:

![Darstellung der Verschlüsselungssituation in Matrix-Räumen](/images/room_security_status_en.png)

