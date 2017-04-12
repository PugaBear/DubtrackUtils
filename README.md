# DubtrackUtils
Hook Dubtrack into your minecraft server!

*Credit to [@sponges](https://github.com/sponges) / [@zombachu](https://github.com/zombachu) for the [Dubtrack4J](https://github.com/zombachu/Dubtrack4J) library*

## Features
- Song update announcements
- Display dubtrack chat in minecraft and vice-versa
- Hide announcements/chat per person
- Kick/ban users from ingame
- Skip the current song from ingame
- [*Fully* customizable](https://github.com/PugaBear/DubtrackUtils/blob/master/src/main/resources/config.yml)- every message and every feature.

### Planned features
- IRC/Discord hooks
- Grab other misc. information about the dubtrack room

## Commands
### Basic
**Permission: dubtrack.use**
- `/dubtrack` - View information about dubtrack, a link, and what is currently playing. 
- `/dubtrack hide [chat]` - Hide announcements or chat (by adding 'chat') 
### Mod
**Permission: dubtrack.mod**
- `/dubtrack kick <user>` - Kick a user from the dubtrack room
- `/dubtrack ban <user>` - Ban a user from the dubtrack room
- ~~/dubtrack unban \<user\> - Unban a user from the dubtrack room~~ Will try to fix later
- `/dubtrack skip` - Skip the current song
### Admin
**Permission: dubtrack.admin**
- `/dubtrack reload` - Reload the configuration file 
- `/dubtrack reconnect` - Reconnect to dubtrack 
- `/dubtrack reset` - Reload the configuration file and reconnect to dubtrack 

## Download
[DubtrackUtils.jar](http://dl.bn-mc.net/?q=dubtrackutils)

## Installing
- Drag and drop into plugins folder
- Stop / start server
- Edit the [config.yml](https://github.com/PugaBear/DubtrackUtils/blob/master/src/main/resources/config.yml)
- `/dubtrack reset`

## Building
You will first need to clone the [Dubtrack4J](https://github.com/PugaBear/Dubtrack4J) library and install it to your local Maven cache.
```
git clone https://github.com/PugaBear/Dubtrack4J.git
cd Dubtrack4J
rm src/test/ -R
mvn clean install
cd ..
git clone https://github.com/PugaBear/DubtrackUtils.git
cd DubtrackUtils
mvn clean package
```
The jar will be inside the `target` folder.

## Contact
### Discord
[<img src="https://discordapp.com/api/guilds/132680070480396288/widget.png?style=shield">](https://discord.gg/0jwsKTH4ATkkN8iB)

or Griffin#2583
### IRC
[#Bear-Nation on irc.spi.gt](http://irc.bn-mc.net)
