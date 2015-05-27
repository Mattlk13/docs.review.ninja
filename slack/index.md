---
layout: default
slack: true
---

## Slack Integration

ReviewNinja can integrate with [Slack](https://slack.com/) to notify through messages when certain events occur!

{% image slack-message.png width="100%" %}

Currently, we support Slack notifications for three different types of events:

* Starring and unstarring a pull request.
* Creating a pull request.
* Merging a pull request.

### Creating a Slack Token

In order to start using ReviewNinja with Slack, you first need to create a Slack API token.

Go to [this link for Slack's web API](https://api.slack.com/web).

Once there, go to the "Authentication" section and click "Create Token" for the team you want ReviewNinja to send messages to. Copy the generated token.

### Setting up a Repo for Slack Notifications

Once you have the token, go to any repo in ReviewNinja and click the Settings icon (the <i class="fa fa-cog"></i>) at the top.

Once in the settings page, at the bottom, there will be a section for Slack Integration:

{% image slack-integration-settings.png width="100%" %}

Paste the generated token from Slack into the "Token" section, give the #channelname that you want in the "Channel" section, and your repo will be good to go.
