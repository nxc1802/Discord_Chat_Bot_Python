# Music bot
Since a lot of discord music bots are being blocked by youtube nowadays I've decided to write up a quick project that will allow anyone to host their own discord bot. This bot includes the following commands:

/help - displays all the available commands
/p <keywords> - finds the song on youtube and plays it in your current channel. Will resume playing the current song if it was paused\
/q - displays the current music queue\
/skip - skips the current song being played\
/clear - Stops the music and clears the queue\
/leave - Disconnected the bot from the voice channel\
/pause - pauses the current song being played or resumes if already paused\
/resume - resumes playing the current song

## How to download it

This repository is now a template, on the top left you can simply click on "**Use this template**" to create a GitHub
repository based on this template.

Alternatively you can do the following:

- Clone/Download the repository
  - To clone it and get the updates you can definitely use the command
    `git clone`
- Create a discord bot [here](https://discord.com/developers/applications)
- Get your bot token
- Invite your bot on servers using the following invite:
  https://discord.com/oauth2/authorize?&client_id=YOUR_APPLICATION_ID_HERE&scope=bot+applications.commands&permissions=PERMISSIONS (
  Replace `YOUR_APPLICATION_ID_HERE` with the application ID and replace `PERMISSIONS` with the required permissions
  your bot needs that it can be get at the bottom of a this
  page https://discord.com/developers/applications/YOUR_APPLICATION_ID_HERE/bot)

# Running with docker
To run with docker simply run the command `docker run -e TOKEN=<your_token_here> -d pabolo02345/music_bot:latest`

# Installation
To run the discord bot all you need is python 3.4 or above.\
Then run `pip install -r requirements.txt` to install all of the python dependencies.\
Please note that you will also need to have [ffmpeg](https://ffmpeg.org/download.html) installed and make sure that the path to the bin folder is in your environment variables. 

# Token
Remember that you need to have your token setup in your environment variables as well and it should be under TOKEN. On windows you can do this by running 
`SET TOKEN=<you_token_here>`
After that you can start it with

```
python bot.py
```

# Built With

- [Python 3.11.5](https://www.python.org/)

