# Terraform -> Discord Webhook Proxy

Have you ever wanted to use the webhook notification system on Terraform to notify a Discord channel of your infrastructure state changes, only to realize that they can't natively talk to each other? Well not anymore, because here's the tool you've been searching for!

_Terraform webhook comes in, Discord webhook goes out, profit._

By default, an embedded rich message will be sent to Discord but this can be disabled in the config file.

![Rich Message](https://i.imgur.com/Q9uNRqV.png)

## Usage

1. Download: `go get github.com/captainGeech42/tf-discord-webhook-proxy`
2. Copy the `config.ex.json` file to your current directory as `config.json`
3. Update the `WebhookURL` field with a Discord webhook URL ([Discord docs on webhooks](https://support.discord.com/hc/en-us/articles/228383668))
4. Run it: `tf-discord-webhook-proxy`