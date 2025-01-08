# Making PRs

This is instructions on how to make PRs (Pull Requests) for submissions of the weekly problems in AD450. 

1. Follow the directions in for [Configure Github with VSCode](https://canvas.seattlecolleges.edu/courses/30109/pages/python-vscode-and-github-setup) to set up this repo. Be sure to follow the directions for copying this repo using the template button. 

2. First make a small edit to a file and save it. Then you will check the status of your github repo by running `git status`. You will run this a lot in this tutorial. This is what I got. Notice I am on the main branch, I made modifications to `week_2_intro_ipython.ipynb` and I have added the file `week_4_panadas.ipynb`. We are going to be working with just the week 2 file in this example.


3. Then create a branch by running the command below with BRANCH_NAME replaced with a reasonable file name for the branch. In the screenshot below I used `week_2_ipython_branch`. I also checked the status of my branch after. You see I am no longer on main but now on `week_2_ipython_branch`.
```
git checkout -b BRANCH_NAME
```

4. Now you will stage the files on your branch with the add command below. Checking the status you can see that not the week 2 file is green. This means it is staged on the branch. The week 4 file is still red because we did not add it to the branch.

```
git add week_2_intro_ipython.ipynb
```

5. Next we will commit the changes with a message. The message is added with the flag `-m` and the message will be whatever follows in quotes.
```
git commit -m "Added first attempt of week 2 problems"
```

6. We will now push our branch to github. I first run `git push`. This will not work the first time to push a new branch but it will give you the command you need. You can see in the output below git gave me the command I needed to push my branch. Yours might look different if you named your branch something else. Run the command git give you and you should get a link. This will be the PR that you open, click the link.

7. This link will open a PR on your branch in your repo. It should be automatically filled out with the PR template in this repo. You will fill out this template before opening your PR.

8. Now let's suppose you made some changes to your code that you want to appear in your PR. Once you have saved your changes run `git status` to see your unstages changes. You will follow steps 4, 5, and 6 again. In step 5 you will use a different commit message to describe your new changes. In step 6 you will just need to run `git push` since you've already created the branch on GitHub.

9. Once you have commited all the code to your branch and pushed it to GitHub you are ready to open your PR. You'll fill out the PR tempated and then click the `Create pull request` button. Once you have done that you will add your instructor and TA as reviewers and submit the link to PR to the assignment in Canvas. If you don't know the GitHub username of the instructor and TA just submit the link to canvas and we will add ourselves as reviewers.

**Congrats on making your first PR!**