ASSIGNMENT 1: STARTING A GIT REPOSITORY

Open a terminal and run these commands one by one:

mkdir html-lab
cd html-lab
git init
git config --local user.name "Your Name"
git config --local user.email "your-email@example.com"
git config user.name
git config user.email

Create index.html with the following content:
<!DOCTYPE html>
<html>
<head><title>HTML Lab</title></head>
<body>
    <h1>Welcome to My HTML Lab</h1>
</body>
</html>

Then run:
git status
git add index.html
git commit -m "Add home page"

Add this heading below the h1 in index.html:
<h2>Next Lab Meeting</h2>

Then run:
git add index.html
git commit -m "Add next meeting heading"
git log --oneline

ASSIGNMENT 2: PUSHING AND CLONING A REPOSITORY

From inside html-lab, run:
git init --bare ../html-remote
git remote add origin ../html-remote
git remote -v

Push your branch. If your branch is main:
git push origin main

If your branch is master:
git push origin master

Then run:
cd ..
git clone html-remote html-copy
cd html-copy
git log --oneline

NOTE: Git terminal outputs depend on your computer, Git version, and branch name.
Take your own terminal screenshots after running the commands.
