# Bot Commands

Thespian uses Discord's new Slash Commands feature. To get a list of all the commands available, just type `/` in any channel in your server. 

## `/character`

This contains subcommands related to Thespian characters.

### `/character create [name] [prefix] [optional: avatar_url]`

Create a character. Thespian will create the character, then DM you a link, which you can use to edit the character's bio and adjust settings.

You'll supply a name, and a [prefix](/prefixes.md).

Optionally, you can supply a URL for the character's avatar to set it right away. You can change it later with `/character edit`.

### `/character delete [name] [are_you_sure]`

Delete one of your characters by name. There's a second input called `are_you_sure` which _has_ to be `True` for the command to work. Deleting a character is *permanent*, and cannot be undone.

### `/character edit [name] [optional: regenerate]`

Thespian will DM you a unique link you can visit to edit your character. Be careful! The link can be used by _anyone_ to edit your character, so don't share it. 

If you want to invalidate any old unique links and create a new one, you can use the optional `regenerate` argument.

### `/character list [optional: page] [optional: dm]`

List all of your own characters. You can optionally pick which page you list, or whether to send it to yourself in a DM instead of in a public channel.

### `/character search [name]`

Search for characters in the current server. This will search for approximate name matches of characters that belong to other users in the server.

This will _only_ search for characters that are flagged as 'public' and would already appear on your user page. If you don't want your character to show up in searches, be sure to turn off 'public' when editing them.

## `/permissions`

This contains subcommands related to permissions. You can whitelist, or blacklist, certain channels or roles from using Thespian's character-posting functionality.

## `/permissions show`

Show the current state of all permissions in the server

## `/permissions default [op]`

Set whether the server allows character posting by default. This is global, across all channels and all roles.

## `/permissions role [op]`

Set whether users with a specific role can post as their characters. This overrides the default setting.

## `/permissions channel`

Set whether users in a specific channel can post as their characters. This overrides the default setting.

## `/permissions manager set`

Set the role that is the assigned _manager_ of permissions. Users with this role can use all `/permissions` commands.

## `/permissions manager clear`

Un-set the manager role.

## `/invite`

Get an invite link to the Thespian bot to add it to your own server!