---
title: "Terms of use"
date: 2024-02-16T14:00:00+01:00
draft: false
chapter: true
---

# Terms of use

These terms of use come into force on 08.04.2024.

## Deletion deadlines

### Notes on the Federation

{{% notice note %}}
Data or files stored on other matrix servers cannot be deleted by TU Dresden. Members of TU Dresden can use the federation to access rooms on external matrix servers and vice versa. In this case, the external server also holds data and files from the TUD matrix server, but may handle the deletion of this information differently. It is also possible that data is still available in the temporary cache of users' Matrix clients.
{{% /notice %}}

### Files

Matrix can be used to exchange files, but is not intended for longer-term storage. For this reason, files that have been received or sent in Matrix are automatically removed from the TU Dresden Matrix server after a certain period of time. Specifically, a file is deleted 12 months after it was last accessed.

{{% notice tip %}}
Appropriate services such as [Datashare](https://tu-dresden.de/zih/dienste/service-katalog/zusammenarbeiten-und-forschen/datenaustausch/cloudstore) can be used for the permanent storage of files.
{{% /notice %}}

### Sessions

Sessions that have not been used for more than 120 days are automatically deleted. You will therefore be logged out of the Matrix client you are using.

{{% notice info %}}
When you log in to a Matrix client such as Element, a session is created. Logging out of a session deletes it. Sessions can be viewed in Element, for example, via "Settings" - "Sessions". Inactive sessions, i.e. sessions that have not been used for a long time, are listed separately in this view and can be removed if necessary.
{{% /notice %}}

{{% notice tip %}}
In general, you should only log out of a session if "Secure Backup" is enabled or the "E2E room keys" were exported before logging out and at least one more is available. This ensures that access to encrypted messages is still possible.
{{% /notice %}}

### Matrix accounts

#### With inactive ZIH login

If the ZIH login has expired, existing sessions are deleted. This means that you will be logged out of all Matrix clients in use. Access to the Matrix account is not possible with an expired ZIH login. 

If the ZIH login is reactivated within 15 months, access to the Matrix account is possible again. However, there may be restrictions on access to encrypted messages:

* Access to encrypted messages received during inactivity is not possible.
* Access to older encrypted messages is only possible if either
  * the "Secure Backup" is active and its security key or phrase is known or
  * the "E2E room keys" were exported before the ZIH login expired.

#### If ZIH login is blocked

If the ZIH login has been expired for more than 15 months, the associated Matrix account will be deactivated.

The following Matrix account data will be deleted:

* memberships in all rooms
* all sessions
* all E2EE keys
* the "Secure Backup"
* display name
* profile picture
* block list

The following data is not deleted:

* uploaded files
* Sent and received messages
