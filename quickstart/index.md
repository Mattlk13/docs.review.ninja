---
layout: default
quickstart: true
---

## Quickstart

The steps below detail how to get up and running with ReviewNinja, including a description on the basic workflow and philosophy behind a ReviewNinja code review.

### Add your repository

{% image add-repo.png width="100%" %}

To add a repository to ReviewNinja hit <i class="fa fa-plus-circle"></i> to reveal the search dialog, here you may search for a repository.

To remove a repository, click <i class="fa fa-times"></i>.

### Basic Workflow

ReviewNinja is a code review tool built for pull requests. We suggest adopting the [Git Flow Workflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow), but ReviewNinja can be adapted for any workflow as long as pull requests are used.

ReviewNinja provides two mechanisms for conducting code review. [**Ninja stars**](/stars) indicate approval, and [**review flags**](/codereview) specify a specific problem that needs to be resolved before the pull request should be merged.

> **ProTip:** ReviewNinja integrates well into the [GitHub Flow](https://guides.github.com/introduction/flow/index.html).

### Merge with Confidence

The Merge Pull Request button changes color to indicate the level of confidence in the merge.

{% image pull-good.png width="33%" class="pull-left" %}

{% image pull-pending.png width="33%" class="pull-left" %}

{% image pull-bad.png width="33%" %}


### Ignoring files

A ``.ninjaignore`` file specifies which files should be ignored by ReviewNinja. Each line specifies a file pattern, just like a [.gitignore file](http://git-scm.com/docs/gitignore).

Please note, ignored files will be minimized by default and still available for inspection in ReviewNinja.


### Collaboration

Keep track your team's activity via the Team Tab. The Team Tab displays each collaborator and their contributions, including the number of ninja stars added, number of threads opened and the number of pull requests merged.

The Team Tab also allows you to invite repository collaborators to ReviewNinja.

