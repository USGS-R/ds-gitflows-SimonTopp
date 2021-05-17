Welcome to the end of the hands on tutorial with Git and GitHub! You have now been exposed and practiced the basic workflow that USGS DS uses for collaborating on codebases. See the bottom of this issue for instructions about next steps.

## The conceptual diagram of the workflow you just learned/used 

![image](https://user-images.githubusercontent.com/13220910/81212707-dfc22680-8f9a-11ea-8fc8-ad0d960d8207.png)

## A summary list of commands that were used.

### Setting up a new project

1. Fork the canonical repo to your username.
1. Create a local copy of your fork - copy the SSH URL from **your fork's** GitHub page, then in Git Bash run `git clone [insert your fork's SSH URL]`.
1. Add the canonical repo as a remote to your local version - copy the SSH URL from **the canonical repo's** GitHub page, then in Git Bash run `git remote add upstream [insert canonical repo's SSH URL]`.
1. Verify that you are ready to go with remotes - run `git remote -v` and check that your fork's URL is next to `origin` and the canonical repo is listed next to `upstream`.

### Saving a change locally

1. Change the file(s).
1. Inspect what changes git detects - run `git status`
1. Stage the files that you want to include in your commit - `git add [insert file name]`. Pro tip: use `git add .` to stage all changed files listed with `git status`.
1. Commit your staged changes - `git commit -m "[commit message here]"`

### Moving your local commits to your fork

1. Run `git push origin master`
1. Look at the "commits" page on your fork on GitHub to see your new commits.

### Adding your changes to the canonical repository

1. Once you have changes on your fork that make it different from the canonical repository, go to your fork's GitHub page and click "New pull request". 
1. In the next screen, verify that the `base` repository shows the canonical and the `head` repository shows your fork. 
1. Click "Create pull request".
1. Add a title and description. Include a peer as a reviewer and link to any related issues by adding `#[issue number]` in your description.
1. The reviewer will merge the changes.
1. Close the loop by pulling down the changes from upstream to your local repo - `git pull upstream master`

### Handling merge conflicts

1. If you have a merge conflict after pulling down changes, look in the file(s) that have been flagged as having conflicts.
1. Inspect the content between `<<<<<<< HEAD` and `=======`, which is the content that existed before the merge (likely your content).
1. Now inspect the content between `=======` and `>>>>>>> [string of letters and numbers]`, which is the content that is trying to be merged with what currently exists locally (likely the remote content).
1. Decide what of that content to keep and what to delete.
1. Remove the merge conflict symbols, `<<<<<<< HEAD`, `=======`, and `>>>>>>> [string of letters and numbers]`.
1. Save the file and then commit your merge resolution (see above for making commits). The the message "resolve merge conflict" is often used.

## Feeling confident? Explore more!

There is a lot more Git that can be learned, but the above are the basics that will probably be enough for awhile. As you start to get more advanced, there may be some additional concepts/commands you should learn such as, 

* Temporarily hiding changes in order to pull upstream changes to avoid conflicts (`git stash`, `git stash apply`),
* branching (`git checkout -b`), and
* much more!

----
**Action:** Once you are done reading this, close this issue and return to the canonical repo's main GitHub page `https://github.com/USGS-R/ds-gitflows-[username]`.
