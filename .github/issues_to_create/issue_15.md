Your PR was merged! Yay! Now, remember that "closing the loop" thing we did after our last PR was merged? Let's do it again.

Merging a PR creates a commit on the canonical repository. Even though the most recent changes were your additions, technically your fork and local repository do not have that "merge" commit and are now out-of-date with the canonical repo. So, we need to close the loop.

----
**Action:** Close the loop. 

1. Open Git Bash and make sure you are in your project's directory (reminder: use `cd`).
1. Pull down changes from the canonical repository (aka the "upstream" remote) by running `git pull upstream master`.
1. We now have changes locally that do not appear on our fork (aka the "origin" remote). So if we run `git status`, we get the message "Your branch is ahead of 'origin/master' by X commits".
1. Just like we did earlier, we can push our local changes to our fork by running `git push` (or `git push origin master` to be explicit).
1. Now when you run `git status`, you should see that everything is up-to-date and there is nothing to commit. 

You have once again closed the loop after your PR was merged! Close this issue and move to the next one.
