We refer to online versions of GitHub repositories as "remotes". If you open Git Bash to your project directory (you may need to `cd ds-gitflows-[username]` from the end of the last issue) and run `git remote -v`, you will see a list of remotes and their URLs that are currently associated with your local copy. Currently, you have one remote - your fork of the repository - though you will see both a fetch and push option for it. It is referred to as the `origin` because your local copy *originated* from it. 

What we need to do now is link the canonical repository to your local copy. This closes the loop and enables you to pull down changes that collaborators have merged to the main repo into your local version. We refer to the online canonical version as the `upstream` repo and it is a `remote` because it is online.

----
**Action:** Link your cloned repository to the upstream remote.

1. Open the GitHub page for the main (or canonical) repository, `https://github.com/USGS-R/ds-gitflows-[username]`
2. Just like in the previous step, click `Clone or download`
3. Copy the SSH URL (not the HTTPS URL)
4. Open Git Bash to your project's working directory.  
5. Type `git remote add upstream [insert URL]`, e.g. `git remote add upstream https://github.com/USGS-R/ds-gitflows-[username]`. *Reminder:* you cannot CTRL+V to paste into Git Bash. Right click and choose paste instead.
6. Hit enter.
7. Now, when you run `git remote -v` you should see a list with both an `upstream` remote and an `origin` remote.

You have now set up your new project for collaborative development! We are ready to start making changes. Close this issue and move on to the next one.
