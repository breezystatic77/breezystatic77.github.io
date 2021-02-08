# Bot Commands

You can send a command to a bot by mentioning it, starting the comand with `th!`, or by sending it a private message.

You can include the arguments for the command in the initial message, or just type the command, and the bot will ask for more information.

## `help`

**Also:** `h`

DMs you a list of all commands. Similar to this page.

## `avatar`

**Also:** `a`

Change or add a character's avatar. This is the picture that appears next to messages by them.

You supply the character's name, and attach a file to be used as an avatar. Smaller, square images work best.

#### Example

```
th!avatar "Billy Bob" (attach an image)
```

## `create`

**Also:** `c`

Create a character. Thespian will create the character, then DM you a link, which you can use to edit the character's bio and adjust settings.

You'll supply a name, and a [prefix](/prefixes.md).

#### Example

```
th!create "Billy Bob" ++TEXT
```

## `edit`

**Also:** `e`

Get Thespian to DM you the _private_ link you can use to edit your character. Be careful about sharing this link - anybody who has access to it can also edit your character. You can use the `regenerate` command to create a new link.

## `info`

**Also:** `i`

Get Thespian to respond to your message with a link to one of your characters.

You'll supply a name. (Advanced use: you can also supply any character's UUID, instead)

#### Example

```
th!info Aragorn
```

?> To get info about a character from one of their messages, react to a (recent) message from them with a ❓. Thespian will DM you a message. [More info](reactions#❓)

## `list`

**Also:** `l`

Get a list of all your characters.

This will only show characters you list as showing up on your user page. To get a list of _all_ characters, use this command in a PM with the Thespian bot.

---

## `permissions`

**Also:** `p`

Show all the permission settings for the current server.

## `permission-default`

**Also:** `pd`

Edit what a default permission is for @everyone.

## `permission-channel`

**Also:** `pc`

Edit a permission for a particular channel.

## `permission-role`

**Also:** `pr`

Edit a permission for a particular server role.
