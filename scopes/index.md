---
layout: default
scope: true
---

## ReviewNinja's Use of GitHub's OAuth Scope

ReviewNinja authenticates all sessions with GitHub's provided OAuth service. We never store code in our own data persistence. We do store user tokens (provided by OAuth), and id (GitHub's unique id). All other information stored is specific to ReviewNinja. ReviewNinja is a "client-heavy" application, meaning that every request for GitHub data is piped to GitHub and subject to their security mechanisms.

The following are the activities that ReviewNinja does with the GitHub permissions:

  1. Set commit statuses
  2. Read the primary email address of the user
  3. Create and delete webhooks
  4. Retrieve all repositories of a user

ReviewNinja requests the following permissions:  

 * `user:email`

	Allows ReviewNinja to use a user's email address to send notifications. ReviewNinja does not store a user's email in its perisistance.

 * `repo`

	Allows ReviewNinja to access a user's repository commit diffs, files, issues, and Pull Requests in order to perform a code review.

 * `repo:status`

	Allows ReviewNinja to update a commit's status.

 * `read:repo_hook`

	Allows ReviewNinja to read from a repositories webhooks.

 * `write:repo_hook`

	Allows ReviewNinja to write to a repositories webhooks.

 * `read:org`

	Allows ReviewNinja to read from the organizations to which you belong.

Please refer to [GitHub's API documentation](https://developer.github.com/v3/oauth/#scopes) for more information.
