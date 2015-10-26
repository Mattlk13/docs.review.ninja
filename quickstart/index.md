---
layout: default
quickstart: true
---

## Quickstart

Go to <a href="http://app.review.ninja/auth/github" target="_blank">ReviewNinja</a> and authenticate with GitHub.  If you are wondering what ReviewNinja needs those permissions for,  please refer to the [GitHub OAuth Scope](/scopes) documentation page.

### Add your repository

{% image add-repo.png width="100%" %}

To add a repository to ReviewNinja hit <i class="fa fa-plus-circle"></i> to reveal the search dialog.

Start searching for the repository.

> **Hint:** You must search by owner/repository. 
> For example to find ``review.ninja`` you would search for ``reviewninja/review.ninja``

To remove a repository, click <i class="fa fa-times"></i>.

### Basic Workflow

Code Review is accomplished using two features:

  * [**Review Comment Threads**](/codereview) - comment threads opened up on individual lines of code with flags to indicate if issues in the code have been resolved or not.
  * [**Ninja Stars**](/stars) - markers of approval on a pull request.

  Basic workflow would be:

  1. Create a branch for your feature.
  2. Commit.
  3. Submit a Pull Request.
  4. Collaborators of the project review the code and create review comment threads or ninja star the code as a sign of approval.
  5. The collaborators decide if sufficient code review has occurred and merge the Pull Request.

> **ProTip:** ReviewNinja integrates well into the [GitHub Flow](https://guides.github.com/introduction/flow/index.html).

### Merge with Confidence

The Merge Pull Request button changes color to signal the level of confidence in the merge.

{% image pull-good.png width="35%"%}

If the number of ninja stars reaches the defined threshold and there are no open review comment threads, the Merge Pull Request button appears green.  

{% image pull-pending.png width="35%" %}

If there are no stars, the Merge Pull Request button appears orange.  

{% image pull-bad.png width="35%" %}

If there are open review comment threads, the Merge Pull Request button appears red.


### Ignoring files

A ``.ninjaignore`` file specifies which files should be ignored by ReviewNinja. Each line specifies a file pattern, just like your  [.gitignore file](http://git-scm.com/docs/gitignore).

Please note, ignored files will be minimized by default and still available for inspection in ReviewNinja.


### Collaboration

Keep track your team's activity via the Team Tab. The Team Tab displays each collaborator and their contributions. Including # of ninja stars added, # of threads opened and the # of merged Pull Requests.

The Team Tab also allows you to invite repository collaborators that have not yet joined ReviewNinja. 

