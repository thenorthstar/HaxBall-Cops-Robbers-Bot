# HaxBall-Cops-Robbers-Bot
Cops and Robbers bot HaxBall players

<a href="https://discord.gg/t6Wvbqk"><img alt="Discord" src="https://img.shields.io/discord/536193210096156682?color=blue&label=DEVELOPER%27S%20DISCORD"></a>

## Getting Started
This bot is a hard-coded advanced level Cops & Robbers bot for HaxBall players and coders. In past some trials for creating a Cops & Robbers bot was performed - like yellow - but we couldn't had seen a regular opening one. Now here's a candidate for this. Before introducing the bot, let me remind that for some performance reasons, circle filling functions will be updated later.

## What is Cops & Robbers
Cops & Robbers is a game in which the players separated into teams (mostly blues are more crowded than reds, but here not) and blues try to catch (in here we call arrest or bust) reds and win the game; whereas reds a.k.a. robbers try to stay alive against blues. Now let's what rules this game has:

### Rules

* Game ends when there are no robbers in the pitch. Teams are swapped after game ends.
* In most of the rooms, leaning at the corners is prohibited as it causes the robber to stay alive after collisions.
* In most of the rooms, more than a certain amount of players on gate is not allowed.
* It's prohibited for everyone to collide with their teammates.
* Players can use discs to get hidden from other teams (i.e. a robber can get hidden from cops not to get busted).
* Robbers have possibility to back to pitch as many as possible if there's at least one robber in the pitch.
* Time limit is usually 3 minutes.

After informing about rules, without further ado, let's move to what this bot has as innovation:

* When game is being ended, the swapping operation is done automatically.
* To lean at the corners (only for robbers) for more than 3 seconds and keep staying inside discs (for both teams) for more than 10 seconds result in an automatic ban. This means less load for administrators during the game. By the way, this room doesn't need an administrator at all.
* In this room, only one player from cops is allowed to stay on gate (this may also done dynamic according to the amount of robbers against the cop).
* Like yellows, this bot also has the feature to make the players are transparent to each other. As default, all the players are free to collide others as physically but it's possible to make it impossible by a simple command (see **commands**).
* Robbers will be teleported at the lock-up zone after collisions (in transparent mode, the collision between cops and robbers is made by script as HaxBall API doesn't allow to collision between the additional **cGroup**s like **c0**, **c1** and etc).
* Time limit here is 3 minutes as default but can be edited.
* Not yet ended, in collision-open mode, there will be only one player who is allowed to enter in a single disc (under construction).
* After each game ends, players gain or lose points as their status.
* Player admin status, ID and points are visible to others on chat section. Also players will stay in knowledge of the time.
* And the most important thing, some important room objects meet all these stuff above (to avoid more work when editing the code).

Now, let's move to commands after talking about what news are:

### Commands
In contrary of other bots, this room has so simple commands. In the beginning we were planning to build this bot with more languages but we have left the bot in 2 languages (Turkish and English) as before, due to some timing and translation problems. Now let's take a look at commands. By the way, commands are different in both the languages:

* !admin (The same as in English): Get/leave admin rights.
* !afk (The same as in English): Set/unset AFK.
* !bb (The same as in English): To get kicked by see off message.
* !collision (**!çarpışma** in Turkish): To turn on/off the collision feature. If on, players are free to collide, otherwise the players are transparent to each other.
* !commands (**!komutlar** in Turkish): To see the available commands.
* !dc/!discord (The same as in English): Get discord address of the room (This can be edited by user).
* !lang (**!dil** in Turkish): The command for changing your language while in the room (**en** and **tr** are available codes).
* !stats (**!istatistikler** in Turkish): To see your statistics (i.e. how many times you lost in robbers etc.). By the way, a new feature is under construction for **statistics**. Stay tuned...

## Notes
Before finishing, let's remind some important notes of course:

* Like the previous ones, this bot is also licensed and it's strictly prohibited to sell it by cost and share it anywhere without the author's permission.
* Some features may not always be added. This means the user should work and do what they want as his own. If so, you can get help from the scripts in the following link whenever you want: https://github.com/thenorthstar/HaxBall-Example-Scripts
