Time to add on to this story. We've done this a couple times now, so the edit-save-add-commit pattern should be getting familiar.

----
**Action:** Add text for the next two sections and commit those changes.

1. If you run `git status` in Git Bash  right now, you should see a message that says "nothing to commit" and also "Your branch is ahead of 'origin/master' by 1 commit" (that one commit is the one from your collaborator that has not yet been pushed to your fork). 
1. Open the `dryville_story.md` file on your computer and add the next section of [the story](https://www.usgs.gov/special-topic/water-science-school/science/story-water-dryville), which is called "Your First Flood". Keep the same formatting as before (`##` for the title, `[inline text](url)` for hyperlinks). Save the file.
1. If you run `git status` in Git Bash, you should see the words "modified: dryville_story.md". This means that Git detects your change. You will also see the words "no changes added to commit". This is because we still need to stage our changes. Note that you will still see "Your branch is ahead of 'origin/master' by 1 commit" - we still haven't pushed since we pulled down our collaborator's changes.
1. Run `git add dryville_story.md` to stage these changes so that they can be included in our next commit. Now when you run `git status`, you see that the "modified: dryville_story.md" change is listed under "Changes to be committed". We are now ready to make a commit.
1. Run `git commit -m "add your-first-flood section"` to make a commit.
1. Run `git status` again. We should be back to where we started. There is "nothing to commit" because we don't have any additional changes to the repository content - we already committed our changes. However, you will now see that it says "Your branch is ahead of 'origin/master' by 2 commits".
1. Now repeat for "Storing Water for a Rainy Day". Copy and paste text from [the complete story](https://www.usgs.gov/special-topic/water-science-school/science/story-water-dryville). Keep the same formatting as before (`##` for the title, `[inline text](url)` for hyperlinks). Save the file.
1. Run `git add dryville_story.md` to stage these changes.
1. Run `git commit -m "add storing-water-for-a-rainy-day section"` to make a commit.
1. Now `git status` shows that we are ahead of `origin/master` by 3 commits.

You have now made two new commits. Close this issue and move on to the next one.
