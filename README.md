# Seed Repo
Welcome to CS249r! This repository will house the assignments.

If you are reading this, the name of the repository should be ```assignments-YourGithubID```. If that's what you see, you should already be logged into your Github account and have your own private repository (this one) for your assignments. You're good to read on.

If you don't see your Github ID at the end of the repository name, you need to follow [this link to Github Classroom](https://classroom.github.com/a/_hZODl1X) to create your own private repository.

If you don't know what any of this means please see the tips for getting GitHub setup below and if you need any additional help please reach out to the course staff!

## How this repository works
This repository is a copy of a "seed" repository maintained by the TFs. Throughout this semester, your TFs will add assignments to the seed repository, and you will be responsible for copying them into your local repository (using ```fetch``` and ```merge```, in git-speak). Assuming you've already cloned your repository locally using the Github Classroom link, you can get new files for subsequent assignemnts:
```
git remote add seed_repo https://github.com/Harvard-CS249R-Fall2020/assignments.git # only needs to be done once
git fetch seed_repo
git merge seed_repo/master -m "Fetched new assignment" --allow-unrelated-histories
```
These commands:
1. Tell your local git repository where the seed repo is (and calls it ```seed_repo```),
2. Get that repo from github.com,
3. And merge it with your local files. 

## Some tips for getting GitHub setup (if you haven't used it before)
1. Install git on your computer if you haven't already. For Linux/Mac OSX you can use ```apt-get``` or ```homebrew``` to install (e.g., ```sudo apt-get install git```). For windows you can use the [GitHub Desktop Client](https://desktop.github.com/) or [download](https://git-scm.com/downloads) and install it directly
2. Create a [GitHub](https://github.com) account. We suggest using [ssh](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/) over https.
3. We strongly encourage you to learn git instead of simply using the github website. Here are some useful links for interested students: [Harvard/SEAS](https://wiki.harvard.edu/confluence/display/USERDOCS/Introduction+To+GIT), [Github tutorials](https://help.github.com/articles/good-resources-for-learning-git-and-github/), [Git Cheatsheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet).

At a very high level: Use ```git clone``` to get a copy of the repository on your own machine. Use ```git fetch``` and ```git merge``` to access new assignments and updates. When you are ready to submit your work, use ```git status``` or ```git diff``` (to check and analyze for uncommited changes) and ```git add --all```, ```git commit -m "msg"``` to save work and ```git push``` to send to the server (and ```git pull``` to download from the server).
