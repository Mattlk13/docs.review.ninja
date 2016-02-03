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

Head to your repo and click on the <i class="fa fa-cog"></i> icon. From here
simply click on the "Add to Slack" button, specify a channel, specify events
and you're good to go!

Be sure to include the '#' or '@' when specifying a slack channel or DM
respectively.
