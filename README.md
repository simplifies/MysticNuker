# MysticNuker

## Dependencies

Please install the `requests` library using `pip install requests` if you have not already done so. If the program shuts down immediately after starting, check that you have requests installed using `pip list`.

## How to set up MysticNuker

Put your token and your settings into `config.json`:

- `token`: Your discord token. If you do not have your discord token, look up how to get it on YouTube.

- `webhook_name`: The username that webhooks created by the nuker should have.

- `webhook_content`: The message that you want spammed when a webhook nuke is done.

- `spam_per_webhook`: Number of messages to send for each webhook. There is a limit of 50 webhooks for a server and the bot will make one webhook for every channel until it reaches the maximum. The recommended value is 10, which will potentially send ~500 pings to the your server.

- `chan_nuke_amount`: Number of channels to create in a nuke. Recommended value is 250 but it can go as high as 500.

- `chan_nuke_name`: Name that you want the created channels to have.

- `global_thread_count`: Use this to edit the number of threads the program operates on. 50 is the default value, and anything higher is really unnecessary because of discord ratelimiting. Edit at your own risk.

## How to use MysticNuker

Simply run `MysticNuker.py`. You will be prompted to give the ID of the Server you want to nuke. Once it confirms that the guild is valid, you can select one of the following options:

- DelChannels - Delete all channels in the server.

- MakeChannels - Create the channels defined in `config.json`.

- Webhooks - Create webhooks in a server if they do not already exist, and then spam them.

- Nuke - Use all three of the above methods in a row.

- Exit - Close the Program

If you find any bugs or have requests for more features, send me a message on Discord or open up a new issue on this repository. I hope you enjoy!
