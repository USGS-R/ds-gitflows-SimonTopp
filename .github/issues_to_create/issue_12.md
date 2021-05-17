In the last issue, we made two commits that added two new sections of the story to our `dryville_story.md` file. Huzzah! Everything is peachy. However, while you were doing that, your collaborator also decided to add to the story and they committed before you. Now, we need to once again pull down their changes before moving on.

----
**Action:** Pull down your collaborator's most recent additions. 

1. First, verify that you did indeed close the previous issue.
1. Before pulling down changes, verify that you don't have any uncommitted changes locally. Run `git status` and look for the phrase, "nothing to commit".
1. Next, pull their changes down using `git pull upstream master`. 
1. Uh oh, there seems to be an issue. When we pulled down those changes, the message "CONFLICT (content): Merge conflict in dryville_story.md" appeared. We must have been editing the same line of the file as our collaborator.

Your first merge conflict! Everything will be OK, promise :) Close this issue and move on to the next one.
