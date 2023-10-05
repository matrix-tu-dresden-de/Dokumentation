---
title: "Messages"
date: 2020-07-15T18:10:07+02:00
draft: false
chapter: true
weight: 30
---

## Find people and send direct messages

To write to individuals and thus create a 1:1 chat, first click on the + in the category "Direct messages":

![Click on the Start Chat button](/images/01_Start-Chat_en.png)

Now start typing the email address of the person you want to find in the search field.

People who already have a matrix account can also be found by their display name (usually "first name last name"). Please wait up to five seconds after the last entered character until the search results are displayed. Persons who have not yet logged in can only be found via their e-mail address or their ZIH login. The link button "Show More" will display further search results. Please also note the server on which the searched person is displayed.

{{% notice note %}}
Inserting e-mail addresses (e.g. via Ctrl+V) is usually not sufficient to find people! Please enter the characters of the e-mail address by hand, character by character and wait up to five seconds until all hits are displayed.
{{% /notice %}}

If you cannot find anyone, ask for their username, share your username (@ZIH-Login:tu-dresden.de) or https://matrix.to/#/@_Your_ZIH-Login_:tu-dresden.de, so that the person addressed can contact you within Matrix. An invitation e-mail is not sent by Matrix.

![Result added to the people invited to the chat](/images/99_Find-Neo_de.gif)

Note that Matrix accounts may not be checked by ZIH function logins. Due to the novelty of the medium for many and the missing multi-account functionality of the Matrix client element, TU Dresden employees may prefer to use their personal ZIH login.

In the search result, click on the target person and then on "Go":

![A search result for the search query entered](/images/04_Found-and-Go_en.png)

The [end-to-end encrypted]({{< relref "encryption" >}}) (meanwhile standard) conversation opens, which can begin after the connected person accepts the invitation. The connection to the server at the TU Dresden is of course also transport-encrypted. If you explicitly do not want end-to-end encryption for a special reason, [create]({{< relref "rooms/create.en.md" >}}) an unencrypted room and invite the conversation partners to it.

### Invite a group of persons

For the mass invitation of persons (up to 100 at once, then repeatable) the matrix names are necessary, which should be in the form `@ZIH-Login:tu-dresden.de`. Collect them e.g. in a text editor line by line and then paste them into the search field in Matrix/Element using the clipboard (copy & paste).

### Using a room as a clipboard

It is possible to create a room with yourself. In this room you are the only participant. This room can then be used as a clipboard / notebook as well as for tests, for example to check whether formatting (for example of latex) and hyperlinks work correctly.

### Further reading
* [formatting messages]({{< relref "formatting.en.md" >}})
* [searching messages]({{< relref "search.en.md" >}})
