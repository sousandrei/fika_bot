[![Main](https://github.com/sousandrei/fika_bot/actions/workflows/main.yaml/badge.svg)](https://github.com/sousandrei/fika_bot/actions/workflows/main.yaml)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Fika Bot

FikaBot is a simple Slack bot to match two random people in a channel so they can have some [Fika](https://sweden.se/culture-traditions/fika)!

## Usage

First you are going to need a Slack application. FikaBot needs the following permissions

```
- commands
- im:write
- users:write
- channels:read
```

On top of that, you'll need to create two slash commands, all pointing to a `/commands` url

```
/fika_start
/fika_stop
```

The application needs 2 environment variables to function!

```sh
SLACK_TOKEN='xoxb-......'
MONGO_URL='mongodb://127.0.0.1'
```

`SLACK_TOKEN` Is the bot token of your slack application, denotet by starting with `xoxb`

`MONGO_URL` is the mongo connection string for the bot to store it's data

Provide the application with those as enviroment variables and you are good to go!

## Building

No secret here

```bash
cargo build --release
```

## Contributing

Don't hesitate to ask for features and open PR's.
