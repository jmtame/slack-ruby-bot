## Installation

Create a new Bot Integration under [services/new/bot](http://slack.com/services/new/bot).

![](screenshots/register-bot.png)

On the next screen, note the API token.

### Environment

#### SLACK_API_TOKEN

Set SLACK_API_TOKEN from the Bot integration settings on Slack.

```
heroku config:add SLACK_API_TOKEN=...
```

#### SLACK_RUBY_BOT_ALIASES

Optional names for this bot.

```
heroku config:add SLACK_RUBY_BOT_ALIASES=":pong: table-tennis ping-pong"
```

### Heroku Idling

Heroku free tier applications will idle. Either pay 7$ a month for the hobby dyno or use [UptimeRobot](http://uptimerobot.com) or similar to prevent your instance from sleeping or pay for a production dyno.
