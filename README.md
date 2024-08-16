# tg_captcha_go

Telegram bot that validates new users that enter supergroup. Validation works like a simple captcha. Bot written in Go (Golang).

## How it works

1. Add the bot to your supergroup
2. Promote the bot for administrator privileges
3. A new user enters your supergroup
4. Bot restricts the user's ability to send messages
5. Bot shows a welcome message and a captcha button to the user
6. If the user doesn't press the button within 30 seconds then the user is banned by the bot

## If you want to run your own instance of the bot

- [Option 3](./INSTALL-3.md): systemd

## Commands

`/healthz` - check that the bot is working correctly

## Сustomization

You can change several bot's settings (welcome message, ban duration, socks5 proxy server) through the configuration file `config.toml`

## copy from Forks
- [mxssl/tg-captcha-bot](https://github.com/mxssl/tg-captcha-bot/tree/master) 
- [momai/tg-captcha-bot](https://github.com/momai/tg-captcha-bot) - fork of `tg-captcha-bot` with interesting additional features.

go mod tidy
go run 
