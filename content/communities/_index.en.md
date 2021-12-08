---
title: "Communities"
date: 2020-07-02T21:22:34+02:00
draft: false
chapter: true
weight: 50
---

# Communities (deprecated)

{{% notice note %}}
[Spaces]({{< relref "spaces/_index.en.md" >}}) replace communities for room management. The feature is automatically enabled in current Element versions. (Desktop/Web 1.9, Android 1.3, iPadOS/iOS 1.6 or later)
{{% /notice %}}

## Content
  * [Show Communities temporarily](#show-communities-temporarily)
  * [Convert Communities](#convert-communities)
  * [Use Communities as room filters](#use-communities-as-room-filters)

## Show Communities temporarily

![Selection of "All settings" item in the user menu](/images/06_Settings_en.png)

Click on the downward pointing arrow at the top right of the people column and call up `All settings`.

![Element settings with preferences to Communities](/images/20_Communities_Settings1_en.png)

In the dialog on the left, select `Preferences` (1). On the right side, under the heading `Communities`, you will find the option `Display Communities instead of Spaces` (2). If you activate the slider to the right, your Element client will be reloaded and the Communities will be displayed. Click the slider again if you want to return to the regular view.

## Convert Communities

![Selection of "All settings" item in the user menu](/images/06_Settings_en.png)

Click on the downward pointing arrow at the top right of the people column and access `All settings`.

![Element settings with preferences to Communities](/images/20_Communities_Settings2_en.png)

In the dialog on the left, select `Preferences` (1). On the right side you will find the entry `Show my Communities` (2) under the heading `Communities`. Unfold the entry and your Communities will be displayed. With a click on the button `Create Space` (3) to the right of each entry the conversion dialog is called.

![Dialog für die Konvertierung einer Community zu einem Space](/images/20_Communities_Conversion1_en.png)

Here you can configure the photo, the name, the description and the visibility (private or public) of the Space. Afterwards the conversion can be started with a click on `Create Space`.

![Dialog with success message after conversion](/images/20_Communities_Conversion2_en.png)

Once the process is complete, you will receive a success message. The `Preferences` button will take you back to the Communities settings.

## Use Communities as room filters

All matrix users of the client element (and a few other clients) can use communities to filter different rooms, which may be lost or scattered in the room list on the left.

Communities can only be created for yourself or for others (if you invite them into a community) and create a superordinate structure for rooms. For example, for a semester group/study group or for a chair team etc.

Existing rooms can be assigned to a community in the community settings (under #).

![Screenshot of the selection of the current community](/images/20_Communities.webp)

A community created with the + button can be drag'n'dropped from the community avatar (little picture) onto the sidebar.

A small HTML page can be used to describe the community.

Unfortunately it is currently not possible to add more administrators through the matrix client: [https://github.com/vector-im/element-web/issues/5240](https://github.com/vector-im/element-web/issues/5240)

Removing rooms from communities is done by clicking on the hash # in the upper right corner, then clicking on the room to be removed and then clicking on "Remove from community".

A community can be deleted when the administrator leaves it.

### other administrators

Currently no more administrators can be added to a community via Element. Issue on Github](https://github.com/vector-im/riot-web/issues/5240) If you need more administrators in a community, they can be added by the Matrix Admin Team. Please send a support request to servicedesk@tu-dresden.de.

