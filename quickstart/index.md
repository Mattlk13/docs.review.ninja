---
layout: default
quickstart: true
---

## Quickstart

Go to <a href="http://review.ninja/auth/github" target="_blank">ReviewNinja</a>
and authenticate with GitHub. If you are wondering, what ReviewNinja needs
those permissions for, please refer to the [GitHub OAuth Scope](/scopes)
documentation page.

### Add your repository

{% image add-repo.png width="100%" %}

To add a reposion tory to ReviewNinja hit <i class="fa fa-plus-circle"></i> to
reveal the search dialog.

Start searching for the repository.

> **Hint:** The search is repository scoped, not owner. When you have the
> repository `reviewninja/review.ninja`, then you only need to search for
> `review.ninja`

ReviewNinja loads the repositories that you have write permissions for. Select
the the repository you want to add and click the add repo button.

To remove a repository, click <i class="fa fa-times"></i>.

### Basic Workflow

  1. Create a branch for your feature.
  2. Commit.
  3. Submit a pull request.
  4. Collaborators of the project review the code and create issues or star the
     code as a sign of approval.
  5. If issues were opened, they are fixed. Goto 4.
  6. The collaborators decide if sufficient code review has occurred and merge
     the pull request.

> **ProTip:** ReviewNinja integrates well into the [GitHub
> Flow](https://guides.github.com/introduction/flow/index.html).

### Code Review

Click the repository you want to view. All pending pull requests of this
repository appear in a list.  

Click a pull request to begin a code review.

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
where and what needs fixing. When collaborators looks at that pull request,
they will notice the line tagged with an issue symbol. Once the tagged line
is clicked, the corresponding issue will be opened. In case of several issues
linking to one line, all issues involved are filtered.

Click on other issues to view them, add comments, or close the issues. The
corresponding GitHub issue will also be closed.  

### Ninja Starring

ReviewNinja understands that often in code review what matters most is *who*
did the review. By starring a pull request, it shows that the reviewer has seen
the code change and has approved it.

To star a review, click the ninja <i class="fa fa-star ng-scope"></i>.

### Merge with Confidence

The Merge pull request button changes color to signal the level of confidence
in the merge.

{% image pull-good.png width="200px" %}

If there is at least one star with no open issues, the Merge pull request
button appears green.  

{% image pull-pending.png width="200px"  %}

If there are no stars, the Merge pull request button appears orange.  

{% image pull-bad.png width="200px"  %}

If there are open issues, the Merge pull request button appears red.


### Configuration

You can change your notification settings for pull requests, issues, and stars.
In contrast to GitHub, ReviewNinja email notifications are "opt-in".  You will
only receive email notifications if you select the appropriate checkboxes. 

To configure your settings, click <i class="fa fa-cog"></i>.

You can choose to receive email notifications for the following:

  * Pull requests
  * Issues
  * Ninja stars

You can also enter specific branches that you want to "watch".  You will
receive email notifications about the branch whenever there is an action
related to it.

> **ProTip** Watched branches are not plain text. You can use a wildcard
> to select several branches at once. E.g. "feature/\*"


### Ignoring files

A ``.ninjaignore`` file specifies which files should be ignored by ReviewNinja.
Each line specifies a file pattern, just like your 
[.gitignore file](http://git-scm.com/docs/gitignore).

Please note, ignored files will be minimized and still available for inspection
in ReviewNinja.
