![](https://repository-images.githubusercontent.com/286907609/eb884086-46d8-44bf-95c1-fc2ed8362122) 


# DingoLingo
A Discord music bot written in Python with support for Youtube, SoundCloud, Spotify, Bandcamp, Twitter, and custom files.

### Keep in mind:
* The Wiki may have the answer you are looking for https://github.com/Raptor123471/DingoLingo/wiki
* Known problems are listed in Issues. If you are interested in this project feel free to submit an Issue.


<h3>What's Coming?</h1>

  - See TODO in Projects tab

## Prerequisites:

#### API Keys
* Discord - https://discord.com/developers
* Spotify (optional) - https://developer.spotify.com/dashboard/
  - Client ID
  - Client Secret
  - Note: Limited to 50 playlist items without API

Obtained keys must be entered into ```config/config.py```

#### Requirements

* Installation of Python 3.7+

Install dependancies:
```
pip install -r requirements.txt
```
* Located in ```/config```

For Linux:
* ffmpeg
* libffi-dev 
* libnacl-dev 

### Installing - Self hosting

1. Download release if available, alternatively download repository zip
2. Complete Prerequisites
3. Start ```run.py``` in project root
4. See configuration options in /config/config.py

Button play plugin:
* Set emoji with the setting command to enable this feature
* Emote must be in same server as bot
* Needs Manage Message permissions

Custom Cookies:
* Extract cookies.txt from you browser using your preferred method
* Overwrite the existing cookies.txt in /config/cookies/
* (Optional) Set a custom cookies.txt location by modifying COOKIE_PATH in config.py

## Commands:

### Music

After the bot has joined your server, use ```d!help``` to display help and command information.


```
d!p [link/video title/key words/playlist-link/soundcloud link/spotify link/bandcamp link/twitter link]
```

* Plays the audio of supported website
    - A link to the video (https://ww...)
    - The title of a video ex. (Gennifer Flowers - Fever Dolls)
    - A link to a YouTube playlist
* If a song is playing, it will be added to queue

#### Playlist Commands

```
d!skip / d!s
```

* Skips the current song and plays next in queue.

```
d!q
```

* Show the list of songs in queue

```
d!shuffle / d!sh
```

* Shuffle the queue

```
d!l / d!loop
```

* Loop the current playing song, toggle on/off

```
d!mv / d!move
```

* Move song position in queue

#### Audio Commands

```
d!pause
```

* Pauses the current song.

```
d!resume
```

* Resumes the paused song.

```
d!prev
```

* Goes back one song and plays the last song again.

```
d!np
```

* Shows more details about the current song.

```
d!volume / d!vol
```

* Adjust the volume 1-100%
* Pass no arguments for current volume

```
d!stop / d!st
```
* Stops the current song and clears the playqueue.


### General

```
d!settings / d!setting / d!set
```
* No Arguments: Lists server settings
* Arguments: (setting) (value)
* Use "unset" as an argument to reset a setting
* Example: d!setting start_voice_channel ChannelName
* Administrators only

```
d!c
```

* Connects the bot to the user's voice channel

```
d!cc
```

* Switch the bot to the user's voice channel

```
d!dc
```

* Disconnects the bot from the current voice channel

```
d!history
```
* Shows you the titles of the X last played songs. Configurable in config.config.py


### Utility

```
d!reset / d!rs
```

* Disconnect and reconnect to the voice channel

```
d!ping
```

* Test bot connectivity

```
d!addbot
```

* Displays information on how to add the bot to another server of yours.

## License

This program is free software: you can redistribute it and/or modify
it under the terms of the [GNU General Public License](LICENSE.txt) as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.


## Acknowledgments

https://github.com/adriansteffan/DiscordJockey
