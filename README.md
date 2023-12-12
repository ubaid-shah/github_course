# GitHub Course
This is a complete GitHub course by Ubaid Shah

# Type 1: GitHub-Local-GitHub
- In this type we first create a repo on GitHub and then clone it on local machine.
- After modifying the existing files and/or adding new files we'll push the changes to GitHub origin repository.

## Step 1: Sign Up on GitHub
- Sign Up on  https://github.com/
- Create a new public git  hub repo
## Step 2: Create a New Repo
## Step 3: Download and Install Git
 - Download Git from https://git-scm.com/download/
 - Install it on your local machine or laptop
## Step 4: Git Configuration
- open the git bash and set up the user name using
  
  `git config --global user.name <"your user name">`
- Set up user email
  
  `git config --global user.email <"email_address">`
- Check the details

  `git config --list`

## Step 5: Clone the Github repo
- Go to code on github and click on local the select the https and copy the path of your repo. e.g. `https://github.com/example_git-user/eaxmple_github_repo.git`

- Next create a folder in your laptop and go inside it by 

  `cd <C:\Users\username\folder>`

- Next in the gitbash terminal paste

  `git clone <https://github.com/example_git-user/eaxmple_github_repo.git>`

- Next go inside the github repo

  `cd <example_github_repo>/`

- Now check what's inside the repo

  `ls`

- To check all files and folders including hidden item in the repo

  `ls -a`

- Check the git status 

  `git status`

  Shows the current state of your repository, including **tracked** and **untracked files**, **modified files**,**unmodified**,**staged** and branch information

- Create a new text file

  `touch <new.txt>`

  and add some lines in it.

## Step 6: Add files in Staging area
- Add all modified and new files to the staging area.

  `git add .`

  now check the git status, it will show *Changes to be committed* message with new and modified file names

-  if you want to add only a specific file to staging area then type

  `git add <filename>`

- if you want to unstage all files after staging then type

  `git restore --staged .`    -- it is for all staged files

  `git restore --staged <file1> <file2> ...... `  -- it is for specific files

-  After modifying all files it is mandetory to add it to staging area for commit

## Step 7: Commit the changes
- Now commit the changes
  
  `git commit -m "message"`

  Creates a new commit with the changes in the staging area and opens the default text editor for adding a commit message.

## Step 8: Push the files to GitHub repo
- Now it's time to push all the modified files  to the GitHub repo

  `git push origin main`

# Type 2: Local-GitHub
- In this type we first create a repo on local machine and then push it on GitHub origin After modifying the existing files and/or adding new files.

## Step 1: Create a directory in local machine
- Create a project directory in local machine by any method. 
- To create the directory in desired location using git bash type following code

  `cd <"path of the folder">`

  `mkdir <directory_name>`

-  if you want to rename the directory name before init

  `mv <old_name> <new_name>`

## Step 2: Initialize the git 
- Initialize a new Git repository in the current directory.

  `cd <directory>/`

  `git init`

  it will initialize the git repo by creating a `.git` folder inside it.

  Check it by `ls -a` command

## Step 3: Create new files
- create new files and folders in it
-  if you want to Move or rename a file, a directory, or a symlink after init

  `git mv <old_name> <new_name>`

## Step 4:  Create a new GitHub repo
- Create a new repository on GitHub
- Add remote origin repo

  `git remote add origin <github_repo_url> `

- To verify the branches of remote repo and local repo

  `git remote -V`

- Check the name of the branch

  `git branch`

  This is a `master` branch. Change it's name to `main`

  `git branch -M main`

## Step 5: Push the files to GitHub repo
- Add files to staging area

  `git add .`

- commit the changes

  `git commit -m <message>`

- Push the files

  `git push -u origin main`

  Pushes local commits to the remote repository.

  



