# GitDemo
To demonstrate git push / branch / merge

This to create a workflow guide for Git

# Setting up Git username
1. git config --global user.name
2. git config --global user.email

# Adding and Committing
Step 1: in 'src' folder, run git init
        Or git clone url 

Step 2: git add filename
Optional: git diff // shows the changes, press 'q' at end to quit

Step 3: git commit -m "message"

# Branching
Step 1: create a new branch at the current commmit
    git branch [branch-name]

Step 2: Switching to another branch
    git checkout [branch-name]

Step 3: Merge branch into current one
    git merge [branch-name]

# Pushing to Repo
Step 1: Add alias of project
    git remote add [alias] [url]

Step 2: To push local commits 
    git push [alias/url] [branch]

