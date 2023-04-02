
# Slack Bot

We are going to develop a Slack Bot and configure it according to our need.



## API Reference

#### Get all items to configure the bot

```bash
  SLACK_SIGNING_SECRET
```

| Parameter              | Type     | Description                |
| :--------              | :------- | :------------------------- |
| `SLACK_SIGNING_SECRET` | `string` | **Required**. Your signin secret|

#### Get item

```bash
  SLACK_BOT_TOKEN
```

| Parameter        | Type     | Description                   |
| :--------        | :------- | :-----------------------------|
| `SLACK_BOT_TOKEN` | `string` | **Required**. Token generated |


## Installation

To start with this project run

```bash
npm install dotenv axios @slack/bolt
```

I am using https://replit.com/ to host my project where I will add my index.js file and run it to generate a url.

Create a  `.env` file and add

```bash
SLACK_SIGNING_SECRET=Your_secret
SLACK_BOT_TOKEN=Your_token
```
or add them as secrets in your project at https://replit.com/ and run to get a url.

In `Slack > Event Subscriptions` enable the `Enable Events` and the add
```bash
your_url/slack/events
```

After that in your Slack dashboard select the project and try to type something which include joke or quote keyword and see the magic.
