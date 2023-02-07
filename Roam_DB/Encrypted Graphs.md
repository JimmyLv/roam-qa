## Limitations of encrypted graphs

### Warning #.bg-red-200

If you forget your password for an encrypted graph

**We cannot retrieve or reset it, and we cannot recover your encrypted notes**

[[roam/js]] extensions running in an encrypted graph will have access to the unencrypted data

If you want to be sure your notes are secure **do not use** [[roam/js]] extensions that you did not write yourself

[[Quick Capture]] is disabled

Existing graphs cannot be encrypted

We recommend creating a new encrypted graph and importing the existing graph, then delete the existing graph

Backups and [[Export]]s of the graph are **not encrypted**

Backups and exports currently do not contain the unencrypted images and media files

We hope to add this in the future

[[Offline Graph]]s on the desktop app do not encrypt the images / media files you upload

The media files are stored on your computer, unencrypted

You can still share an encrypted graph with someone else, but they need the password used to encrypt it to access the graph

In the future we hope to release the ability to have multiple password to a graph

Load times of encrypted graphs may be longer than non encrypted

Future features, such as a backend API, may not be available for encrypted graphs

We designed it with the backend API in mind, but likely many of the features of it will not be possible for encrypted graphs

More Info

Images and media files are encrypted only on hosted graphs

This may effect the load time of them

[[Offline Graph]]s on the desktop app do not encrypt the images / media files you upload

Roam only encrypts blocks, pages, and media files

Some metadata about your graph is not encrypted

For example whether block text is centered or a heading is not encrypted, but the actual content of the block is

[[Developer]]

These keys are encrypted

`:user/display-name :user/email :create/email :edit/email :node/title :block/string :user/uid :user/photo-url :entity/attrs :block/props :ent/emojis :user/settings`

How do I change my password?

In the settings panel

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FZwq0lx1Ply.png?alt=media&token=f9b59eb8-6d4e-47e8-a95d-c351a4451ca5)

How do I create an encrypted graph?

{{[[video]]: https://www.loom.com/share/5f7cea684d154559a16d0167cd53f93b}}

How can I verify that my graph is encrypted?

{{[[video]]: https://www.loom.com/share/338bd42b80b647aaa0bed3082c53dccd}}

