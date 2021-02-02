# GitDemo
To demonstrate git push / branch / merge

This to create a workflow guide for Git

# Setting up Git username
```shell
git config --global user.name
git config --global user.email
```

# Adding and Committing
Step 1: in 'src' folder, run git init
        Or git clone url 

Step 2: git add filename
Additional notes:
git add . => adds all files in folder
git add -A => stage all changes
git diff => shows the changes, press 'q' at end to quit

Step 3: git commit -m "message"

# Branching
Step 1: create a new branch at the current commmit
```shell
git branch [branch-name]
```
Step 2: Switching to another branch
```shell
git checkout [branch-name]
```

Step 3: Merge branch into current one
```shell
git merge [branch-name]
```

# Pushing to Repo
Step 1: Add alias of project
```shell
git remote add [alias] [url]
git remote add origin [url]
```
    
Step 2: To push local commits
```shell
git push [alias/url] [branch]
git push -u origin main
``` 

# Contributing to Open Source
Step 1: Create a "fork" of the project by clicking "Fork" button. 
        A copy of the project will now be in your repository.
Step 2: Clone the "fork" 
```shell
git clone [url]
```
Step 3: Set up "origin" remote
        Usually, the "origin" tag is already set up when you clone the fork. 
To check current remotes:
```shell
git remote -v
```
To set "origin" remote: 
```shell
git remote add origin [url]
```
Step 4: Add project repo as "upstream"
```shell
git remote add upstream [url]
```

Now that we have finished our fork process. Let's note the work flow of updating source codes. 
Step 1: Pull latest changes from "upstream"
```shell
git pull upstream master
```

Step 2: Create your own branch
```shell
git checkout -b [branch_name]
```
To check your branches:
```shell
git branch
```

Step 3: Add and Commit your changes
```shell
git add -A
git commit -m "Description of changes"
```

Step 4: Push change to your branch
```shell
git push origin [branch_name]
```

Step 5: Pull Request
After reviewing project guidelines, click "Create Pull Request". 

Step 6: Delete local branch
After the project merges your changes, delete your local branch. 
First switch to master branch, then delete the branch.
Lastly, pull the latest changes from the upstream.
```shell
git checkout master
git branch -D [branch_name]
git pull upstream master
```