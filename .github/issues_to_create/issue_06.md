Practice makes perfect - let's make a second commit to our local repo.

----
**Action:** Add the next section's text and commit this change.

1. If you run `git status` in Git Bash  right now, you should see a message that says "nothing to commit" and also "Your branch is ahead of 'origin/master' by 1 commit". 
1. Open the `dryville_story.md` file on your computer and add the next section of [the story](https://www.usgs.gov/special-topic/water-science-school/science/story-water-dryville), which is called "Dryville's First Water Works". Keep the same formatting as before (`##` for the title, `[inline text](url)` for hyperlinks). Save the file.
1. We have now made a second change in our local repo. If you run `git status` in Git Bash, you should see the words "modified: dryville_story.md". This means that Git detects your change. You will also see the words "no changes added to commit". This is because we still need to stage our changes. Note that you will still see "Your branch is ahead of 'origin/master' by 1 commit" - more on that later.
1. Run `git add dryville_story.md` to stage these changes so that they can be included in our next commit. Now when you run `git status`, you see that the "modified: dryville_story.md" change is listed under "Changes to be committed". We are now ready to make a commit.
1. Run `git commit -m "add dryvilles-first-water-works section"` to make a second commit.
1. Run `git status` again. We should be back to where we started. There is "nothing to commit" because we don't have any additional changes to the repository content - we already committed our changes. However, you will now see that it says "Your branch is ahead of 'origin/master' by 2 commits". We'll talk about that next.

You have now made two commits and recorded your changes with Git! Close this issue and move on to the next one.
