Scenario: You are pointed to a code repository on GitHub (this one) for a project that you just joined. You need to start contributing to this codebase. Where do you start? 

So far in the GitHub lessons, you've learned about using GitHub for version control to make and save changes (commit) and merge those changes into the code (pull request). You were also taught how to use branches to keep your code separate from the canonical codebase. However, that is not the only workflow that can be followed when using Git and GitHub. In our group, we use a slightly different version in order to manage collaborative development. Below is a generic depiction of our version control workflow. It is known more widely as the "fork-and-pull workflow".

![image](https://user-images.githubusercontent.com/13220910/81212295-4bf05a80-8f9a-11ea-8302-99a231f61480.png)

There is a main version of the code that people are collaboratively developing. Each contributor has their own version of this code online and locally. Changes are made locally, sent to their online version, and then combined with the collaborative version of the code. Contributors are able to get the changes from other users by syncing their local version with the collaborative version of the code. Now let's look at that workflow using Git + GitHub terminology.

![image](https://user-images.githubusercontent.com/13220910/81212707-dfc22680-8f9a-11ea-8fc8-ad0d960d8207.png)

There is a main version of the code that people are collaboratively developing (`upstream repository`). Each contributor has their own version of this code online (`forked repository`) and locally (`cloned repository`). Changes are saved locally (`commit`), sent to their online version (`pushed to their fork`), and then combined with the collaborative version of the code (`merged with a pull request`). Contributors are able to get the changes from other users by syncing their local version with the collaborative version of the code (`pull the upstream repository`).

We are going to walk through each of these steps within the workflow in this lesson. We will also learn about merge conflicts and what a `.gitignore` file is all about. 

----
**Action:** Close this issue after you read about the workflow and proceed to the next issue in sequential order.
