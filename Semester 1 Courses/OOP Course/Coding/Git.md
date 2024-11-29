Links: [Git Notion Notes](https://videotutorials.notion.site/Introduction-to-Git-ac396a0697704709a12b6a0e545db049)


# Terminology

Note: Git and GitHub are two completely different tools.
## Repository 
Think of a Git repository (or “repo” for short) as a project folder where all your files and the history of changes are stored (version control). Repositories can exist locally on your computer (local repository) or remotely on platforms like GitHub (remote repository).
## Git 
At its core, Git is a distributed version control system (DVCS). Picture it as a remarkably clever time machine for your code. 

In fact, there are two ways to interact with Git:
1. via a graphical interface, such as within a specific Integrated Development Environment (IDE);
2. via the Terminal (Git Bash).
## Clone

## Fork

## Commit 
When you make changes to files in your repository, you save those changes with a commit. A commit is like a snapshot of your project at a specific point in time. Each commit has a unique identifier and a message describing what you changed.
- A commit is like a checkpoint.
- Allows for version control. Lets you keep a version history of the files in the project.

## Push 
When you use push, you send your local commits to the remote repository. This updates the remote version with your changes, making them available to others.
## Pull 
Pull is the opposite of push. It allows you to fetch and integrate changes from the remote repository into your local repository. This ensures you have the latest updates from others working on the same project.
## Merge 
When you want to combine changes from one branch into another, you use merge. This takes all the changes from a branch and integrates them into the target branch. If there are conflicts (like changes made to the same line), Git will ask you to resolve them.
## Branch 
Git allows you to create branches. A branch is like a separate path for development. You can work on new features or fixes in a branch without affecting the main project. Once you're happy with the changes, you can merge the branch back into the main branch (usually called main or master.
Non-Linear Development: Git introduces the concept of “branches.” Imagine your project as a tree trunk. Branches are like alternate timelines where you can test features, fix bugs, and explore different paths without affecting the main trunk (your stable codebase).

## Fetch



Why combine commit and push?


# Step 1: Installing Git
## Method 1: Using Windows PowerShell
![[Setting up Git-20241003144641130.webp]]



Configuring Your Name & Email:
In your terminal, run the following commands to identify yourself with Git:
``` bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Replace the values inside the quotes with your name and email address. This information is not used to login anywhere, but instead it is used to track who made what changes.

















# Step 2: Initialize a Git Repo 
We need to initialize a repository for the folder that our project is contained in. Otherwise we will get an error like this:

![[Git-20241005082334902.webp|374]]



Open a command prompt and navigate to the folder that contains the project or create an empty folder to start out with.
![[Setting up Git-20241003144707179.webp]]

Once you type `git init`, then open this folder with VS code.

1. Create an empty folder or use an existing project.
2. Open the command prompt.
3. Navigate to this empty folder or project.
4. Type `git init`.
	1. You should see a message “Initialized empty Git repository in `<location>`”.
	2. There should also be a folder named .git. It contains all the necessary files and data that Git needs to manage your project. 
5. Open this folder with VS Code.
6. Back to the command prompt do the rest of the commands it gives you.

```
echo "# CS_Notes" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/jonathank1906/CS_Notes.git
git push -u origin main
```

[Adding New Files | Introduction to Git](https://codefinity.com/courses/v2/7533d91f-0a23-44a3-afc7-c84d5072e189/5aa6942a-dab9-4c0a-a3c4-4e21b6f8fd1b/afe2dd35-4d24-40c5-b82f-6c9f111b1663?openStreakPopUp=true)
# A Typical Git Workflow
FIND A DIAGRAM FOR THIS
1. Modify your code: Work on your project’s files in your working tree, adding, editing, and deleting code as needed.
2. Stage changes: Use Git commands to selectively add modified files or specific portions of files to the staging area.
3. Commit the changes: Create a new commit, encompassing the staged changes. Include a clear and concise commit message.
4. Push to a remote repository (optional): If you’re working with a remote repository on a platform like GitHub, you can ‘push’ your commits to share your work and collaborate.
5. Pull from a remote repository (optional): Retrieve changes (‘pull’) made by others from the remote repository and update your local copy.

# Git Commands


## Adding to the Staging Area
The staging area, also known as the "index", is a file which serves as an intermediate step between your working directory and the Git repository itself. It contains information regarding the changes and files which will be included in the next commit.
This will select all of the red files and add them
``` bash
git add .
```


## How to Commit
1. Add to the stage.
2. 
This will show what changes have been made to the files. It will also show new files which haven’t been added yet.
``` bash
git status
```


This will display a log of the recent changes to files done previously. Its like a log book.
``` bash
git log
```


## Go back to a previous version
``` bash
git checkout <commit-hash>
```

Note each branch has its own history backlog, so if you go to a different branch it will have a different log.
## Go forward to a newer version

## How to Push
- It is required to commit before you can push to the remote repository



## How to create and use Branches


To display the list of branches. This does not create a new branch.
``` bash
git branch
```

To create a new branch:
``` bash
git branch <new-branch-name>
```
To be able to push this newly created branch to the repo:
1. First make sure you are active on the newly created branch using the command the checkout command.
2. Then push using the origin command.



To switch to another branch. The * indicates which branch is active.
``` bash
git checkout <branch-name>
```

Then push by doing
``` git bash
git push origin jonathan
```

when push by 