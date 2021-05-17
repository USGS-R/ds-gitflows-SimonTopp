We are now ready to push our local changes (including the resolved merge conflict) up to our fork (aka remote "origin"). Then, we can open a pull request (PR). 

----
**Action:** Push your changes to your GitHub fork and open a PR. 

1. If you run `git status` in Git Bash  right now, you should see a message that says "nothing to commit" and also "Your branch is ahead of 'origin/master' by X commits". Our local version has new changes that do not appear in our fork (aka the remote `origin` because our local version *originated* from it). 
1. Just as before, we need to "push" our local changes to our remote fork. Run `git push origin master` to do so. 
1. Go to **your fork's** webpage (`https://github.com/[username]/ds-gitflows-[username]`) and click on the `commits` button (see image below). You should see your new commit messages appear there.
1. Now, click the "Code" tab to go back to your fork's home page. At the top, click the "New pull request button".
1. Before your pull request is actually created, you need to verify that you are requesting the correct changes be merged with the correct repository. Remember, we are not working with branches, so don't worry about the fields that say "master". However, you should verify that the `base repository` is set to the project canonical repo (`USGS-R/ds-gitflows-[username]`) and that the `head repository` is set to your fork (`[username]/ds-gitflows-[username]`).
1. After verifying, click the green "Create pull request" button.
1. Add a title to your pull request and a description about your changes. In your description, make sure to reference this issue by typing `#[issue number]`. 
1. Once you add a title and description, click the cog next to the `Reviewers` feature on the right bar and select @lindsayplatt as the reviewer from the drop-down menu. If you do not have the option to add a reviewer, do step 9 and then add the reviewer after.
1. Now, click "Create pull request".

You have successfully made a second pull request! Wait for your PR to be reviewed and merged. Once your PR has been merged, close this issue and move on to the next one.
