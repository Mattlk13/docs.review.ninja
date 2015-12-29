---
layout: default
codereview: true
---

## Review Flags

Review Flags are simply textual comments that indicate a problem that needs to be resolved before a pull request is merged. ReviewNinja parses GitHub's review comments for these flags and sets the pull request status accordingly. The available review flags are as follows:

**To indicate a problem**

<span class="label label-warning">!fix</span>
<span class="label label-warning">!resolve</span>

**To indicate a problem has been resolved**

<span class="label label-primary">!fixed</span>
<span class="label label-primary">!resolved</span>
<span class="label label-primary">!completed</span>

> **ProTip:** Review flag comments can be made on lines of code in either GitHub or ReviewNinja. Collaborators who prefer GitHub can continue to work in their preferred environment and still participate in the code review. If ReviewNinja is used, shortcuts are provided for the creation of review flags. 
