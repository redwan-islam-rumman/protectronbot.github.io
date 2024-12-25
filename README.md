# Welcome to the ProtectronBot Documentation!

This guide will teach you how to install and configure [@protectronbot](http://t.me/protectronbot) for your Telegram group. We'll also explain all of the bot's features. If you have any questions that aren't answered here, please join our support chat: [https://t.me/antispamchat](https://t.me/antispamchat)

## What ProtectronBot Can Do:

ProtectronBot is a powerful Telegram bot designed to keep your group clean, safe, and free from spam. Here's a summary of its capabilities:

*   **Combat Spam:** Automatically removes spam links, shortened URLs, external mentions, forwards, reply keyboard links, and unwanted advertising.
*   **Control Group Messages:** Hide "user joined" and "user left" messages to reduce clutter.
*   **Customize Filtering:** Blacklist specific words and domains to tailor the bot's filtering to your group's needs.
*   **Maintain a Civil Environment:** Detect and remove profanity, and prevent message flooding.
*   **Manage User Permissions:** Restrict permissions for users identified as spammers.
*   **Prevent Bot Invasions:** Stop members from adding spam bots to your group.
*   **We prioritize your privacy and do not share any data with third-party services, such as AI providers, or other external entities.**

## Getting Started: Adding ProtectronBot to Your Group

It's easy to get started with ProtectronBot! Just follow these simple steps:

1.  **Add the Bot:** There are three ways to add ProtectronBot to your group:
   *   **Through Group Settings:**
      *   Go to your group's settings.
      *   Select "Add Member."
      *   Search for "@protectronbot" and add it.
   *   **From the Bot:**
      *   Go to [@protectronbot](http://t.me/protectronbot) and press "Start."
      *   Select "Add ProtectronBot to your group" from the message the bot sends you.
   *   **From Bot Info:**
      *   On the bot's profile page (@protectronbot), click "Add to Group."
      *   Choose your group.
2.  **Grant Administrator Permissions:** Make ProtectronBot an administrator with the following permissions:
   *   **Delete messages**
   *   **Ban users**
3.  **Activate the Bot:** Type `/start` in your group chat to activate ProtectronBot.
4.  **Verify Configuration:** Use the `/status` command to check your settings and ensure the bot is set up correctly.

## Granting Administrator Permissions

After adding the bot, **you must make it an administrator** with the following permissions:

*   **Delete messages**
*   **Ban users**

Once these permissions are granted, type `/start` in your group chat to activate ProtectronBot.

## Checking Bot Status and Configuration

Use the `/status` command to view and change ProtectronBot's settings.

A successful setup will show three green icons in the status message.

*   **First icon (not green):** You haven't made the bot an administrator.
*   **Second icon (not green):** You haven't granted permission to delete messages.
*   **Third icon (not green):** You haven't granted permission to ban users.

You can adjust these permissions in your group's administrator settings.

The `/status` command also shows you which features are currently active. Let's dive into those!

## ProtectronBot Features

### ANTISPAM

*   `/antispam`: This powerful feature automatically detects and deletes spam messages using a neural network. It's designed for quick setup, requiring no manual configuration.
*   `/antispam_mode`: Enable this for stricter filtering. It forces the bot to check messages from all users, including those with a long-standing, trusted presence in the group. Use this if the standard `/antispam` isn't catching everything.

**Managing Users:**

*   **Unban:** `/unban @username` or reply to a user's message with `/unban`.
*   **Ban:** `/ban @username` or reply to a user's message with `/ban`.
*   **Report Missed Spam:** Reply to a suspected spam message with `/report`. The message will be deleted, and your report helps improve the bot's accuracy.

### IMAGEFILTER

*   `/imagefilter`: Protects your group from inappropriate images (erotic content, nudity, sexually suggestive material). This helps avoid potential group blocks due to user complaints. 
   *   Protectron uses its own internal neural network for image analysis, ensuring your data stays private.

### NOEVENTS

*   `/noevents`: Clears out those "user joined" or "user left" messages from Telegram. It's a great way to keep your chat clean, especially in large groups.

### NOLINKS and Similar Functions

*   `/nolinks`:  Blocks all users (except administrators) from posting any links.
   *   **Note:** This is highly recommended to prevent spam and malicious links.

These related functions operate similarly, blocking specific types of content:

*   `/noforwards`: Blocks forwarded messages.
*   `/nolocations`: Blocks messages with location data.
*   `/nocontacts`: Blocks messages sharing contact information.
*   `/nocommands`: Blocks messages containing bot commands.
*   `/nohashtags`: Blocks messages with hashtags.
*   `/novoice`: Blocks voice messages.

### WARNINGBANS

*   `/warningbans`: This feature automatically bans users for repeated rule violations across all groups using ProtectronBot. Use with caution, as it can ban new members who've broken rules in other groups.
   *   **Note** Protectron keeps a global database of rule-breakers, making this feature very effective.
*   **Unban:** Use `/unban @username` or reply to a message with `/unban`.

### NOBOTS

*   `/nobots`: Automatically removes any bots that users try to add to your group. Since bots can't see each other's messages, preventing them from entering is crucial. You'll need to manually remove any bots that are already present.

### ANTIFLOOD

*   `/antiflood`: Enable this if you have users who frequently flood the chat. Excessive messages will be deleted, and a warning about flooding will be issued. If `/warningbans` is active, repeat offenders might be banned.
   *   **Note:** Protectron defines "flood" as sending more than 10 messages per minute.

### PROFANITY

*   `/profanity`: Checks all messages for obscene language. Currently, only English is supported. With `/warningbans` enabled, users can be banned for repeatedly using profanity.

### BLACKLIST and WHITELIST

*   `/blacklist`: Create a list of blocked words, links, or sticker packs.

   *   Add words *without* quotes to block sentences containing them.
   *   Add words *with* quotes to block messages that *exactly* match the quoted word.
   *   Sticker pack names should be in quotes.
   *   `/blacklist_add word1, word2, word3`: Adds multiple words or phrases (comma-separated).
   *   `/blacklist_remove word2`: Removes a specific word.
   *   `/blacklist_clear`: Clears the entire blacklist.

*   `/whitelist`: A list of exceptions to the blacklist. You can add channel names or links. For example, for `t.me/my_channel`, add "my_channel" to the whitelist.
   *   **Note:** The Whitelist is useful for allowing specific links or mentions that might otherwise be blocked.

### WELCOME: Greeting New Users

*   `/welcome`: View the current welcome message.
*   `/welcome_set`: Customize the welcome message.
   *   Use multiple lines (press Ctrl+Enter for a new line).
   *   Include links in this format: `[Link Text](http://example.com)`

    Example: `/welcome_set Welcome to the group! Read the rules here: [Rules](http://example.com/rules)`

   *   **Note:** This demonstrates the use of markdown formatting in the welcome message, specifically using a link as shown in the example above.

## We hope this guide was helpful! Happy moderating!