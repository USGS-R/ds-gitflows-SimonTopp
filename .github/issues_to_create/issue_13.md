In the last issue, we pulled down changes from our collaborator and realized that there was a merge conflict. This occurs when you edit the same line of code. In this case, you both added on to the last line of the file. Don't worry - merge conflicts are not as intimidating as they may seem. Let's do this!

----
**Action:** Fix the merge conflict. 

1. Open your local `dryville_story.md` file.
1. Scroll through the file and look for where the merge conflict happens. Merge conflicts are denoted by `<<<<<<<` at the start and `>>>>>>>` at the end. Sometimes, there are multiple conflicts and each will be sectioned off with the left and right pointing carrots.
1. We have one merge conflict in this situation, so that makes this easier. Merge conflicts happen because Git doesn't know which are the correct lines. A human needs to intervene and decide what to keep and what not to keep. Look at your conflict in `dryville_story.md`. The content between `<<<<<<< HEAD` and `=======` is the content that existed in your version of the file before you attempted to pull other changes. The content between `=======` and `>>>>>>>` is what you pulled down and tried to merge. Examine the differences between the content in those sections.
1. The most obvious difference is that your version has the `Your First Flood` section, while the version you are trying to merge does not. So, you would want to keep the `Your First Flood` text. Cut and paste that section so that it is outside and above the `<<<<<<< HEAD` section (see below).

```
## Your First Flood

You're again happy until the first desert downpour hits. The rain flows down the hills (runoff) into Dryville's town center and suddenly you have your first flood — more unwanted water (and the mud it carries with it) to deal with. You decide to build a set of storm drains to fix this problem. Lay some more (this time BIG) pipes through town with intakes where the water collects in low spots. Storm water will flow into these pipes and be sent on its way downhill into your creek. Another problem solved.

But when the storm hit, Dryville Creek overflowed and flooded some houses that were built on the flood plain, the flat ground alongside of the creek. You can do two things here. Look at the lay of the land and decide what parts of the creek bed will flood most often when it really rains and don't allow people to build houses there, or build a dam upstream to create a reservoir to trap storm water before it floods into town. Your reservoir can then release the water slowly over a long period of time, thus preventing floods and recharging ground water.

<<<<<<< HEAD
## Storing Water for a Rainy Day

You start thinking... a reservoir (you can call it a lake) above town could really serve a lot of purposes. A lake will provide a place for you to have fun — go swimming, boating, catch catfish, and relax. You can run your water-supply intake pipes from the lake instead of from your creek, especially since the flood destroyed your water-intake pumping station. With a dam you can release only the amount of water you want into the creek below the dam, thus making sure you have just the right amount of water running in Dryville Creek at all times. A dam would even help prevent flooding downstream because you can hold extra rainfall and runoff during a storm and slowly release it afterward. You can build a bigger paddle wheel, or, better yet, construct a real [hydroelectric power plant](https://www.usgs.gov/special-topic/water-science-school/science/hydroelectric-power-water-use) in your dam to start generating electricity! More problems solved.
=======
## Storing Water for a Rainy Day

You start thinking... a reservoir (you can call it a lake) above town could really serve a lot of purposes. A lake will provide a place for you to have fun — go swimming, boating, catch catfish, and relax. You can run your water-supply intake pipes from the lake instead of from your creek, especially since the flood destroyed your water-intake pumping station. With a dam you can release only the amount of water you want into the creek below the dam, thus making sure you have just the right amount of water running in Dryville Creek at all times. A dam would even help prevent flooding downstream because you can hold extra rainfall and runoff during a storm and slowly release it afterward. You can build a bigger paddle wheel, or, better yet, construct a real hydroelectric power plant in your dam to start generating electricity! More problems solved.
>>>>>>> afd002e4b66f31f815e4236ffa6ea3e17f127e1d
```

5. Now, continuing on. Examine the differences between the "Storing Water for a Rainy Day" sections. Can you find any?
6. The only difference should be that your version (the top one) has a hyperlink for the hydroelectric power plant, while the version that is being merged does not. So, we actually want to keep only the version that you created. 
7. Delete the content between `=======` and `>>>>>>>`.
8. Now you are left with the merge conflict symbols and the correct version of the "Storing Water for a Rainy Day" section. Delete all of the symbols related to the merge conflict (`<<<<<<< HEAD`, `=======`, and `>>>>>>> [random letters/numbers]`). Now, you should be back to where you started (which happens in merge conflict resolution sometimes).
9. Save the file.
10. The last step for resolving a merge confict is to commit your changes. Follow the same pattern as before. Running `git status` will show you that you have an unresolved merge conflict. Just as before, run `git add dryville_story.md` to stage your changed file. Then commit by running `git commit -m "resolve merge conflict"`. 
11. Now, when you run `git status` you will see that you don't have any changes to commit (but your branch still ahead of origin/master - see next issue).

You successfully resolved a conflict! Close this issue and move on to the next one.
