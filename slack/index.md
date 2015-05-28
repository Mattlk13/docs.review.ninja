---
layout: default
slack: true
---

## Slack Integration

ReviewNinja now supports [Slack](https://slack.com/) integration!

{% image slack-message.png width="100%" %}

Currently we post notifications for these events:

* Starring and unstarring a pull request.
* Creating a pull request.
* Merging a pull request.

### Preparing a Slack Bot for a channel and getting a token.

In order to start using ReviewNinja with Slack, you first need to [create a Slack Bot](https://my.slack.com/services/new/bot).

Choose any user name and click "Add Bot Integration". This will take you to the bot setup page that includes an API token. Copy this token.

In Slack, go to the channel in which you wish to enable ReviewNinja notifications. Click on the encircled <i class="fa fa-info"></i> icon at the top for channel info, then click the "Invite more people to this channel" link. Add the bot you just created to this channel.

### Setting up a Repo for Slack Notifications

When you have created the bot and set it up for your channel, go to your repo in ReviewNinja and click the Settings icon (the <i class="fa fa-cog"></i>) at the top.

Once in the settings page you will notice a section for Slack Integration at the bottom:

{% image slack-integration-settings.png width="100%" %}

Take the token you generated in the previous step when creating the bot and paste into the "Token" section, enter the channel (this is where the notifications will be posted), and tweak which events you wish be notified about.
