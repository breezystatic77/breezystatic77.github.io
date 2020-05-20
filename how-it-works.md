# How Does It Do That?

Thespian uses a technique pioneered by its senior, much-loved bot [Tupperbox](https://github.com/Keterr/Tupperbox), using [Discord Webhooks](https://support.discord.com/hc/en-us/articles/228383668-Intro-to-Webhooks) to make its faux-posts.

When you make a post, Thespian checks if it's got any of the prefixes of any of your characters, and if it does, it deletes the message and posts a Webhook in its place.

Deleting posts and replacing them isn't a new technique - but with Webhooks, it can look like an actual person.

Due to Discord's restrictions on webhooks, Thespian can't do the following:

- Change the username color from white
- Remove the "BOT" tag
