---
layout: default
title: ReviewNinja Use of GitHub API Scopes
---
<h1 id="github-api-scope">
ReviewNinja Use of GitHub API Scopes
</h1>

We authenticate all sessions with GitHub's provided OAuth service.  We never store code in our own data persistence.  We do store user tokens (provided by OAuth), and name (GitHub handle).  All other information stored is specific to ReviewNinja.  ReviewNinja is a "client-heavy" application, meaning that every request for GitHub data is piped to GitHub and subject to their security mechanisms.

The following are the activities that ReviewNinja does with the GitHub permissions:

  1. Create issues
  2. Set statuses
  3. Read the primary email address of the user
  4. Create and delete webhooks

ReviewNinja requests the following permissions:  

 * user:email

	Allows us to use your email address to send you notifications. We do not use your email address for any other purpose, nor do we store your email in our perisistance.

 * repo

 	Allows us to access your repo diffs, files, and pull requests in order to perform a code review.

 * repo:status

 	Allows us to update commit status.

 * read:repo_hook

 	Allows us to read from a repositories webhooks.

 * write:repo_hook

 	Allows us to write to a repositories webhooks.

 * read:org

 	Allows us to read from the organizations to which you belong.

 * write:org

 	Allows us to write to the organizations to which you belong. We use this for creating issues.

Please refer to [GitHub's API documentation](https://developer.github.com/v3/oauth/#scopes) for more information.
