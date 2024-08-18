#LEARN ABOUT GIT AND GITHUB
GIT:
git is version control system use to track files it is free and opensource software
github is an online web based servise to host git repositories you can share your code with others.
To install git visit https://git-scm.com/downloads and select dowload for windows if you are on windows or else you select for your system
COMMANDS OF GIT:
git --version= used to see your git version
repository:repository is just a folder which keeeps your file in language of git we call it repo
git status:displays the status of current working directoory
To conmfig your settings use the following commands:
git config --global user.email "your-email@example.com"
git config --global user.name "Your Name"
To check your config settings use the following commands:
git config --list
HOW TO CREATE A REPO:
to create a respository we need to initialize it using git init command
then we can write our code in the file then add it to staging area using git add command and the we use git commit to make it in repo then we will use git push command to push it on github
we also pass a message when using the git commit command
i.e. git commit -m 'message'
git log=it is used tosee the history of your repos and commit history
it also has a version that is git log -oneline to show oneline details
GIT IGNORE: git ignore is the file that contains the file you want git to ignore
BRANCHES:Branches are a way to work on different versions of a project at the same time. They allow you to create a separate line of development that can be worked on independently of the main branch
head: head is the pointer that point the current branch
COMMAND FOR BRANCHES:
to list all the branches in the current repository we use git branch.
to create a new branch we use git branch branchname.
to switch to the another  branch we use git switch branch name.
To create and switch to a new branch we use the command git switch -c branch name
To merge a branch use git merge branch name 
To rename a branch use git branch -m old-branch-name new-branch-Name(here m is the message you need to pass it could be anything)
to delete a branch use git branch -d branch name
GITT DIF:
It is used to compare the changes made in one commit with the changes made in another commit .
git diff(compares working directory and staging area)
git diff --staged(compare staging area and repository)
git diff branch-name-one branch-name-two(used to compare two branches)
git diff commit-hash-one commit-hash-two(use to compare the two specific commit ids)
GIT STASH:
it is use to save the changes you made to temporary location if you want to save it as temporary and do not want to commit.
git stash(it saves the changes to temporary location)
git stash list(shows the list of stashes)
git stash apply(use to apply the stash)
git stash clear(to clear the stash)
GIT REBASE:
It is  used to change the base of a branch.i.e.(git rebase branch name)
Git reflog:
It is used to show the history of commits
To see specific commit we use  git reflog commit-hashid
Torecover lost commits we use git reset --hard commit-hashid
GITHUB:
TO create github account go to github.com and create a account be entering email and username
to configure your files use the following commands:
git config --global user.email "your-email@example.com"
git config --global user.name "Your Name"
To work on github you need to generate a ssh key first and add it to github else you will not be able to use github.
TO generate ssh key use ssh-keygen -t ed25519 -C "your-email@chaicode.com" conmmand on your git bash terminal then save the key and paste it to github website in ssh key tab.
Check remote url setting:
to check your remote url use git remote -v
To add remote repository  use git remote add origin remote-url
To push the code on github use git push -u origin main
To fetch code from remote url use the following commands
git fetch remote-name
TO PULL THE CODE USE :git pull origin main

