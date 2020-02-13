# discord-stars
A simple Discord bot to reward your server members.

Copyright (c) 2020 Dylan Seidt. Licensed under the MIT License.

## Setup Instructions
[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

- Deploy the app to heroku using the button above. If you are using the free plan, you should [verify your Heroku account](https://devcenter.heroku.com/articles/account-verification).
- Create a new application with a bot user on the [discord developer website](https://discordapp.com/developers/applications/me). Copy the bot user's token.
- Go to your app's `Config Vars` and add in a `DISCORD_TOKEN` key with the value of your bot user's token. Add a `DISCORD_PREFIX` key with your desired command prefix. Under Resources, disable the web dyno and enable the worker dyno.
- Invite the bot to your server. Go to the following URL after replacing the `Client ID` found on the discord bot overview page. [https://discordapp.com/api/oauth2/authorize?client_id=**REPLACE**&permissions=8&scope=bot](https://discordapp.com/api/oauth2/authorize?client_id=CLIENTID&permissions=8&scope=bot)
- Try out the help command by running `prefix help` where prefix is the prefix you defined.
