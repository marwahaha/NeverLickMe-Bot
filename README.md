Pokemon-Showdown-Bot

This repository has been abandoned, and will no longer be updated.  Technical support for for this will no longer be given.  Please refer to https://github.com/sparkychild/FoxieBot/ instead.
====================

A chat bot for [Pokémon Showdown][1]. This bot has a number of commands, some helpful and some less so, as well as the capability to mod. It only reacts to basic offences such as flooding/caps/stretching.

  [1]: http://www.pokemonshowdown.com/
  
Guide
-----

Special features of this bot is the Translation API that allows it to function in many languages.  It also includes many games and features that boTTT didn't have.   This bot is somewhat similar to a Showdown server, in the sense that it has it's own 'bot' moderating it (ResourceMonitor) and a hierarchy of ranks of users to control the bot's activity.
All commands can be disabled, to prevent spam or for development purposes.

The bot is also capable in battling in several metagames.

A pastebin guide to the bot's features can be found [here][6]
  
  [6]: http://pastebin.com/zT0eFG8a
  
data/ranks.txt
--------------

Under the folder data, create a new file called `ranks.txt` and put the following in:

  `~username`

with username being your username, followed by an empty line.

Installation
------------


Pokémon Showdown Bot requires [node.js][2] to run.
This bot has not been tested on every `node.js` version possible, but has the same version requirements as [Pokémon Showdown][3]: either v0.6.3 through v0.8.22, or v0.10.2 and up.
Install `node.js` if you don't have it yet, try the last stable version.

Next up is cloning this bot. This can be done in two ways: cloning it via `git` or downloading as ZIP.
Downloading it as ZIP is the easy and lazy way, but is a lot less handy to update than cloning this repository.

To install dependencies, run:

    npm install

Copy `config-example.js` to `config.js` and edit the needed variables.
To change the commands that the bot responds to, edit `commands.js`.

In the folder 'data', create a file and call it ranks.txt and add '~' plus your name in lowercase letters only (no spaces) on the first line.  This will give you admin priviledges on your bot.

Now, to start the bot, use:

    node main.js

Some information will be shown, and will automatically join the room(s) you specified if no error occurs.

  [2]: http://nodejs.org/
  [3]: https://github.com/Zarel/Pokemon-Showdown
  [4]: https://github.com/RivalNick/PS-Bot/wiki/How-To-set-up-Bot

If any of your commands rely on information normally sent to the Pokémon Showdown Client (e.g. functions that execute based on PM that aren't directly related to normal commands), you will need to make changes to the message method in parser.js under the appropriate case.

Development
-----------

Everyone is more than welcome to contribute to the bot.
However, please refrain from adding more example commands.

Owner:
 - sparkychild

Credits:
 - Morfent (Development)
 - TalkTakesTime (Development)
 - Quinella (Development)

License
-------

Pokémon Showdown Bot is distributed under the terms of the [MIT License][5].

  [5]: https://github.com/Quinella/Pokemon-Showdown-Bot/blob/master/LICENSE
