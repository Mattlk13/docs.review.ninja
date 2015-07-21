---
layout: default
codereview: true
---

## Code Review

ReviewNinja allows you to open review comment threads on individual lines of code and make use of flags to indicate whether or not satisfactory fixes have been made to the code.

Comments made on ReviewNinja will also show up on GitHub, and vice versa.

### Starting Code Review

Click the repository you want to view. All pending Pull Requests of this
repository appear in a list.  

Click a Pull Request to begin a code review.

{% image pull-request.png width="100%" %}

> **ProTip:** Not the Pull Request you were looking for? No problem! Use the search bar in the upper right of the Pull Request list. You can search Author, Title, Number, Branch Name and so on. Give it a try! 

Click on a line of code in a diff to leave a comment and start a review comment thread on that line.

### Flags

ReviewNinja makes use of certain flags in comments in order to indicate whether a thread has been resolved or not.

{% image review-flags.png width="40%" %}

* **!fix**, **!resolve** - indicates that there is still work that needs to be done (red threads)
* **!fixed**, **!resolved**, **!completed** - indicates that the issue in that thread has been resolved (green threads)

To add a flag, you have two options:

1. On the list of review threads, click on the status dropdown of the thread you want to change the status of. This will automatically comment the flag you choose.

	{% image thread-flag.png width="40%" %}

2. When commenting, you can just type the flag you wish to apply to the thread. You can make use of the **Add status** dropdown to append a flag to your comment, too.

	{% image add-flag.png width="40%" %}

