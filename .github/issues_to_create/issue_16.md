The last topic we are going to cover in this tutorial is the `.gitignore` file. These files are used when you have a local file that you don't want to track changes to in a commit or put on GitHub. You simply add the name of the file (including directory structure when applicable) to the `.gitignore` file to have Git *ignore* it (see what they did there?). This practice is often used for intermediate files created by processes within your repo, temporary files, or really large data that need to be stored elsewhere. Additional information about `.gitignore` files can be found in [this article](https://www.pluralsight.com/guides/how-to-use-gitignore-file).

----
**Action:** Add a file and then gitignore it.

1. First, open the `.gitignore` file that is in your local directory using a text editor (for example, Notepad++). It should be completely empty.
1. Next, download [this image](https://prd-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/styles/carousel_large/public/thumbnails/image/wss-wu-dryville.jpg?itok=uxY0Fwj1) (right click and choose "Save image as") and save as `wss-wu-dryville.jpg` in your `ds-gitflows-[username]` folder. 
1. Now in Git Bash, run `ls` to "list" the items in your current working directory. You should see the following: `dryville_story.md`, `README.md` and `wss-wu-dryville.jpg`. Note that the `.gitignore` file doesn't show up with `ls` because it is technically a "hidden" file (starts with a `.`).
1. So, you've added a new file to your repository. Now, run `git status`. Git shows that `wss-wu-dryville.jpg` is an untracked file. We could leave it like that and just try to remember to not commit it, but that seems risky. The more foolproof way is to to add it to the `.gitignore` file.  
1. Add `wss-wu-dryville.jpg` to the `.gitignore` file. Save the file.
1. Now run `git status`. It no longer shows `wss-wu-dryville.jpg` as an untracked file, but instead shows that we have modified `.gitignore`. That is because this file is version controlled - whenever we change it, we push those changes to the master repository so that everyone uses the same one. 
1. Now, commit your changes to `.gitignore` and push to your fork.  
```
git add .gitignore
git commit -m "add downloaded image to gitignore"
git push origin master
```
8. Finally, create a pull request. Make sure to add @lindsayplatt as a reviewer of your PR and reference this issue using `#[issue number]`. Reminder - you can look back at closed issues to follow along with past instructions by clicking "Issues" and then "Closed" on the GitHub page for the canonical repository.

Once you open your PR, wait for it to be reviewed and merged. Once your PR has been merged, close this issue and go to the next one.
