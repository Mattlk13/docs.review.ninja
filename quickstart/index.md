---
layout: default
---

<h1 id="quickstart">Quickstart</h1>

Go to <a href="http://review.ninja/auth/github" target="_blank">ReviewNinja</a>.

Enter your GitHub credentials.

We authenticate all sessions with GitHub's provided OAuth service.  We never store code in our own data persistence.  We do store user tokens (provided by OAuth), name (GitHub handle), and email.  All other information stored is specific to ReviewNinja.

## Add your repository

{% image add-repo.png width="100%" %}

If you have multiple organizations, click on the organization with the repository you want to add.  You must have collaborator or owner status to add the repo.

ReviewNinja loads the repositories that you have write permissions for.  Click on the repository you want to add.

To add a repository, click <i class="fa fa-plus-circle"></i>.  
To remove a repository, click <i class="fa fa-times"></i>.

You can also type the name of the repository and click Enter.

## Basic Workflow

  1. Create a branch for your feature.
  2. Write code.
  3. Submit a pull request.
  4. Other members of the organization review the code and comment or star the code as a sign of approval.
  5. The collaborator decides if sufficient code review has occurred and commits the merge.

## Code Review

Compare diffs and add your comments.  ReviewNinja provides a convenient way to add your comments either for a pull request as a whole or on specific line numbers.

Click the repository you want to view.
All pending pull requests in this repository appear in a list.  

Click a pull request to begin a code review.

{% image pull-request.png width="100%" %}

## Issue Management

Any time you discover something that needs fixing, ReviewNinja opens a GitHub issue. 

To create an issue, click Issues <i class="fa fa-plus"></i>.

You must enter a title for the issue.  Entering a description is optional.  To link the issue to a line number, click the line number.  An icon <span class="octicon octicon-issue-opened text-warning"></span> appears beside the line.

Click on other issues to view them, add comments, or close the issues.  The corresponding GitHub issue will also be closed.  

## Ninja Starring

ReviewNinja understands that often in code review what matters most is *who* did the review.  By starring a pull request, it shows that the reviewer has seen the code change and has approved it.

To star a review, click the ninja <i class="fa fa-star ng-scope"></i>.

## Merge with Confidence

The Merge pull request button changes color to signal the level of confidence in the merge.


{% image green-merge.PNG width="50%" %}

If there is at least one star with no open issues, the Merge pull request button appears green.  

{% image orange-merge.PNG width="50%" %}

If there are no stars, the Merge pull request button appears orange.  

{% image red-merge.PNG width="50%" %}

If there are open issues, the Merge pull request button appears red.


## Configuration

You can change your notification settings for pull requests, issues, and stars.  In contrast to GitHub, ReviewNinja email notifications are "opt-in".  You will only receive email notifications if you select the appropriate checkboxes. 

To configure your settings, click <i class="fa fa-cog"></i>.

You can choose to receive email notifications for the following:

  * Pull requests
  * Issues
  * Ninja stars

You can also enter specific branches that you want to "watch".  You will receive email notifications about the branch whenever there is an action related to it.
