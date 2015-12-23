---
layout: default
stars: true
---

## Ninja Stars

Ninja stars are ReviewNinja's approval mechanism. A simple ninja star acts as 
an indicator that you believe a pull request is ready to be merged.

ReviewNinja is built on meritocracy, wherever you see a ninja star, you will
also a picture of the person who gave that star.

**Note**: Ninja stars are tied to the head commit of a pull request. When
the head commit changes (new commits, rebase, etc.) the ninja stars will be
reset to zero, this is necessary due to the ever-changing nature of a pull
request. In order to avoid re-reviews we suggest clearly indicating when no 
more commits are expected on a pull request, and therefore a review can be
conducted (for example, with labels).

There are a few ways to ninja star a pull request. The simplest method to add 
a ninja star is to click the star button in ReviewNinja.

{% image star-people.png width="40%" %}

Additionally, you can give a ninja star by adding one of the following to a
conversation comment on a pull request in either GitHub or ReviewNinja:
<img src="https://assets-cdn.github.com/images/icons/emoji/unicode/1f44d.png?v5" alt=":+1:" width="24px" />
<img src="https://assets-cdn.github.com/images/icons/emoji/unicode/2b50.png?v5" alt=":star:" width="24px" />
<span class="label label-primary" style="font-size: 80%; font-weight: normal;">!star</span>
<span class="label label-primary" style="font-size: 80%; font-weight: normal;">!ninjastar</span>

### Ninja Star Threshold

In your repo settings in ReviewNinja (<i class="fa fa-cog"></i>), you can define how many ninja stars 
are required for a pull request status to be set to successfull.

### Review Team

If your repo is under an organization, it is possible to specify a review
team. When you specify a review team, anyone may still star a pull request,
however, only stars from members of the review team will count towards the
threshold. Members of the review team are clearly indicated with a <i class="fa fa-check-circle text-success"></i>.

**Note**: It is possible for repo admins to have insufficient permissions
to see the review team (if it is a secret team). Because of this we 
strongly suggest you make the review team visible to all members of your 
organization.

**Note**: If members of the review team prefer starring from GitHub, they
will still need a ReviewNinja account in order for their stars to count 
towards the threshold. Having an account is not necessary if no review 
team has been specified, or the star is from a collaborator who is not on 
the review team.
