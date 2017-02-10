# Modmail for Discord
A bot for [Discord](https://discordapp.com/) that allows users to DM the bot to contact the server's entire mod team.
These DMs get relayed to a modmail server where each user gets their own channel, or "thread".
Moderators and admins can then reply to these threads, and these responses are relayed back to the original user as a DM.

Inspired by Reddit's modmail system.

## Setup
1. Install Node.js 6 or higher
2. Clone or download this repository
3. Create a Discord server to be used as the modmail inbox
4. Copy `config.example.json` to `config.json` and fill in the values
5. Run the bot with `node src/index.js`

## Commands

##### Anywhere on the modmail inbox server
`!logs <user>` Lists previous modmail logs with the specified user  
`!block <user>` Blocks the specified user from using modmail  
`!unblock <user>` Unblocks the specified user from using modmail

##### Inside a modmail thread
`!reply <text>` Sends a reply to the user in the format "(Role) User: text" (alias `!r`)  
`!anonreply <text>` Sends an anonymous reply to the user in the format "Role: text"  
`!close` Closes the modmail thread and saves a log of it  
`!logs` Lists previous modmail logs with this user  
`!block` Blocks the user from using modmail  
`!unblock` Unblocks the user from using modmail