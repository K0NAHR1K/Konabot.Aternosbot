# Aternos-Bot
AFK BOT FOR ATERNOS

DOWNLOAD THE Download.TXT file to get the GoogleDrive file


KONABOT - portable Minecraft bot (Windows)
==========================================

A small bot that joins a Minecraft Java server and stays connected. If it gets
disconnected (server restart, network drop, kick), it waits and rejoins.
Nothing needs to be installed: Node.js is included in this folder.




Simple SETUP:

Download the zip file and extract it anywhere.


Edit the file within "Bot > Konabot.aternos > bot.js." 
Edit it with notepad, or notepad++. Change values: 

const BOT_NAME = 'Konabot';   
Name it if you want. 

const HOST = 'PUT YOUR SERVER IP HERE';  
The IP will look like this. Just change it to yours.

const PORT = 01010;  
Your port should look something like this. Change it to yours



launch file will either be "Start-konabot" 
"Konabot" or inside the "Konabot.aternos" folder. 
A file named "start-konabot.bat" will force launch it




Advanced!

SETUP
-----
1. Unzip the whole folder anywhere (do not run it from inside the zip).
2. Open config.json in Notepad and change:
     "host"      your server address, e.g. myserver.aternos.me
     "port"      your server port (25565 for most servers; Aternos servers
                 often show a different number after the colon)
     "username"  a name for the bot - pick your own, not one that is taken
   Leave "version" as 26.1 unless told otherwise.
3. If your server uses a whitelist, add the bot's name: /whitelist add <name>
4. Start your server, wait until it is online, then double-click
   start-konabot.bat. Keep the window open - closing it stops the bot.


NOTES
-----
- The folder must stay together: bot.js, config.json, node.exe, node_modules
  and start-konabot.bat.
- The bot only runs while this PC is on, awake and online.
- Joining a very new Minecraft version (for example 26.3) needs the ViaVersion
  plugin on the server, because the bot speaks version 26.1.
- Minecraft 26.3 servers kick bots that don't send a "tick_end" packet. bot.js
  includes a workaround for this (see mineflayer issue #4189). Once mineflayer
  officially supports 26.3, it may no longer be needed.
- If the bot gets kicked over and over, check the text printed in the window
  and the server's log before changing anything.
- Many free hosts, including Aternos, have rules about bots that keep a server
  running while nobody is playing. Check your host's rules first. You use this
  at your own risk - the bot's author is not responsible for suspensions or
  bans.
- Do not put passwords or other private information in config.json.


CREDITS AND LICENSES
--------------------
- Built on mineflayer (MIT license): https://github.com/PrismarineJS/mineflayer
- Includes Node.js (node.exe), see its license file if one is included, or
  https://github.com/nodejs/node/blob/main/LICENSE
- Keep any LICENSE files that came inside node_modules and the Node folder.
