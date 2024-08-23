# GIT and GITHUB Guide

## Introduction to Git and GitHub

### Git

Git is a version control system used to track files. It is free and open-source software.

### GitHub

GitHub is an online web-based service to host Git repositories, allowing you to share your code with others.

## Installing Git

To install Git, visit [Git Downloads](https://git-scm.com/downloads) and select "Download for Windows" if you are on Windows. Otherwise, select the appropriate download for your system.

## Git Commands

### Checking Git Version

**git --version**
Used to see your Git version.

#### Configuring Git Settings

To configure your settings, use the following commands on your git-bash:

1. git config --global user.email "your-email@example.com"
2. git config --global user.name "Your Name"

#### HOW TO check your configuration setting

**git config --list**
**Repository**:A repository is just a folder that keeps your files. In Git terminology, we call it a "repo."

## Creating a Repository

- To create a repository, initialize it using the git init command.

* Write your code in the file.

- Add it to the staging area.

* Commit it to the repo.

- Push the code to GitHub

### HOW TO ADD FILE TO STAGING AREA:

USE **git add ** command.

### HOW TO COMMIT THE CODE:

USE **git commit -m "pass your message here"** message is mandatory to pass to tell the git what your wile does or what is its purpose.

#### Viewing Commit History###

USE **git log**:Displays the history of your repos and commit history.It also has a version that shows the the history in one line to view the history in one line use the command (**git log --oneline**)

#### Git Ignore:

.gitignore is a file that contains the files you want Git to ignore.

### Branches:

Branches are a way to work on different versions of a project simultaneously. They allow you to create a separate line of development independent of the main branch.

- **Head**:
  HEAD is the pointer that points to the current branch.

### SOME COMMANDS OF BRANSCHES

- **git branch**:Creates a New Branch

* **git branch branchname**:creates a new branch with branchname.

- **git switch branchname**:switch to the branch with branchname.

* **git switch -c branchname**:creates and switches to the branch with branchname.

- **git merge branchname**: merges the branch(branchname) with current branch.

* **git branch -m old-branch-name new-branch-name**:use to rename the branch.

- **git branch -d branchname**Delete a Branch

### Git Diff Commands:

- **git diff**: compare the difference between two commits.

* **git diff**staged\*\*: compare the changes between last commit and staging area(that are not commited yet)

- **git diff branch-name-one branch-name-two**:Compare difference between two branches

* **git diff commit-hash-one commit-hash-two**:Compare two specific commit where hash is the hash id of the commit

### GIT STASH:

Stash is a way to save your changes in a temporary location.

#### Git Stash Commands:

- **git stash**: This command saves your changes in a temporary location.

* **gitstash list**: you can view the stashes using this command.

- **git stash apply**:This command applies the stash:

* **git stash clear**:You can clear the stash using this command.

### Rebase in Git:

Rebasing is used to change the base of a branch.

- **git rebase branchname**: rebase the branch.

#### Git Reflog:

View the history of commits:

##### git reflog commands:

- **GIT REFLOG**:it is used to view the history of commits . +**git reflog commit-hash**:you can find the specific commit with this(hash is the commit id).
  **\*git reset --hard commit-hash**: this command recovers the lost commits.

# GitHub

## Creating a GitHub Account

To create a GitHub account, go to [ GitHub website ](github.com) and create an account by entering your email and username.

### Configuring GitHub with SSH

To work on GitHub, you need to generate an SSH key and add it to GitHub. Otherwise, you won't be able to use GitHub. -**Generating an SSH Key**Use the following command on your Git Bash terminal:

- ssh-keygen -t ed25519 -C "your-email@chaicode.com"
- Save the key and paste it to the GitHub website in the SSH key tab.

#### Checking Remote URL Settings

- To check your remote URL, use:**git remote -v**

* To add a Remote Repository use the command: **git remote add origin remote-url**

- Pushing Code to GitHub:USE **git push -u origin main**

* Fetching Code from Remote:Use **git fetch remote-name**

- Pulling Code from Remote:Use**git pull origin main**
