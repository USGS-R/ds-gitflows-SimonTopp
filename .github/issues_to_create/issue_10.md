Scenario: After your content was merged, a collaborator tells you that they added additional content. You want to keep working, but you don't want to duplicate anything they did. You now need to pull in their content to your local repository before you continue working. Don't worry, we have done this before. We just need to pull down any new changes from the canonical repository!

----
**Action:** Pull down a collaborator's contributions to the canonical repository. 

1. First, verify that you did indeed close the previous issue.
1. Now, visit that canonical repository on GitHub and look at the commits (go to `https://github.com/USGS-R/ds-gitflows-[username]` and click on "commits"). You should see a new commit that was not created by you. 
1. Click on the commit name to see what changes were made. Looks like your collaborator added the next section of the story! 
1. Our goal is to continue this work and add another section but first, we need to get our collaborator's changes locally. Before pulling down changes, verify that you don't have any uncommitted changes locally. Run `git status` and look for the phrase, "nothing to commit".
1. Next, pull their changes down using `git pull upstream master`. Remember, the "canonical repository" is referred to as the "upstream" remote in git commands.
1. Now when you open your `dryville_story.md` file locally, you should see the "Be Gone, Dirty Water" section is the last in the file. 

Great! You successfully pulled down contributions that someone else on your team made to the repository. Next, we will add another section. Close this issue and move to the next one.
