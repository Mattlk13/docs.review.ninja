---
layout: default
quickstart: true
---

## Quickstart

Go to <a href="http://app.review.ninja/auth/github" target="_blank">ReviewNinja</a> and authenticate with GitHub. 
If you are wondering, what ReviewNinja needs those permissions for 
please refer to the [GitHub OAuth Scope](/scopes) documentation page.

### Add your repository

{% image add-repo.png width="100%" %}

To add a reposion tory to ReviewNinja hit <i class="fa fa-plus-circle"></i> to reveal the search dialog.

Start searching for the repository.

> **Hint:** You must search by owner/repository. 
> For example to find ``review.ninja`` you would search for ``reviewninja/review.ninja``

To remove a repository, click <i class="fa fa-times"></i>.

### Basic Workflow

  1. Create a branch for your feature.
  2. Commit.
  3. Submit a Pull Request.
  4. Collaborators of the project review the code and create issues or 
     ninja star the code as a sign of approval.
  5. The collaborators decide if sufficient code review has occurred and merge
     the Pull Request.

> **ProTip:** ReviewNinja integrates well into the [GitHub Flow](https://guides.github.com/introduction/flow/index.html).

### Code Review

Click the repository you want to view. All pending Pull Requests of this
repository appear in a list.  

Click a Pull Request to begin a code review.

{% image pull-request.png width="100%" %}

### Issue Management

Any time you discover something that needs fixing, ReviewNinja opens a GitHub
issue. 

To create an issue, click Issues <i class="fa fa-plus"></i>.

You must enter a title for the issue. Entering a description is optional. To
link the issue to a line number, click the line number. An icon <span
class="octicon octicon-issue-opened text-warning"></span> appears beside the
line.

You can also tag a line of code to the issue, so you can tell more exactly
where and what needs fixing. When collaborators looks at that Pull Request,
they will notice the line tagged with an issue symbol. Once the tagged line
is clicked, the corresponding issue will be opened. In case of several issues
linking to one line, all issues involved are filtered.

> **ProTip:** You can tag multiple lines with shift+click.

Click on other issues to view them, add comments, or close the issues. The
corresponding GitHub issue will also be closed.  

### Ninja Starring

ReviewNinja understands that often in code review what matters most is *who*
did the review. By starring a Pull Request, it shows that the reviewer has seen
the code change and has approved it.

To star a review, click the ninja <i class="fa fa-star ng-scope"></i>.

### Merge with Confidence

The Merge Pull Request button changes color to signal the level of confidence
in the merge.

{% image pull-good.png width="300px" %}

If the number of ninjs stars reaches the defined threshold and there are no
open issues, the Merge Pull Request button appears green.  

{% image pull-pending.png width="300px"  %}

If there are no stars, the Merge Pull Request button appears orange.  

{% image pull-bad.png width="300px"  %}

If there are open issues, the Merge Pull Request button appears red.


### Ignoring files

A ``.ninjaignore`` file specifies which files should be ignored by ReviewNinja.
Each line specifies a file pattern, just like your 
[.gitignore file](http://git-scm.com/docs/gitignore).

Please note, ignored files will be minimized by default and still available for 
inspection in ReviewNinja.


### Ninja Star Threshold

You can define the number of ninja stars required for your project in order for
the Pull Request to be deemed "successful".

To configure this setting, click <i class="fa fa-cog"></i>. You must specify a 
number between 0 and 99.


### Pull Request comments

You can disable automatic Pull Requests comments in GitHub by clicking <i class="fa fa-cog"></i>,
and deselecting this option.


### Email notifications

You can change your notification settings for Pull Requests, issues, and stars.
In contrast to GitHub, ReviewNinja email notifications are "opt-in".  You will
only receive email notifications if you select the appropriate checkboxes. 

To configure your settings, click <i class="fa fa-cog"></i>.

You can choose to receive email notifications for the following:

  * Pull Requests
  * Issues
  * Ninja stars

You can also enter specific branches that you want to "watch".  You will
receive email notifications about the branch whenever there is an action
related to it.

> **ProTip** You can use a wildcards to specify watched branches, e.g. "feature/\*"
