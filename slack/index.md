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

### Creating a Slack Token

In order to start using ReviewNinja with Slack, you first need to create a Slack API token.

Go to [this link for Slack's web API](https://api.slack.com/web).

Once there, go to the "Authentication" section and click "Create Token" for the team you want ReviewNinja to send messages to. Copy the generated token.

### Setting up a Repo for Slack Notifications

With your Slack token, go to your repo in ReviewNinja and click on the Settings icon (the <i class="fa fa-cog"></i>) at the top.

Once in the settings page you will notice a section for Slack Integration at the bottom:

{% image slack-integration-settings.png width="100%" %}

Now you can paste your Slack token, enter the channel (this is where the notifications will be posted), and tweak which events you wish be notified about.
