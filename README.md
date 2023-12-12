# GitHub Course
This is a complete GitHub course by Ubaid Shah

## Step 1: Sign Up on GitHub
- Sign Up on  https://github.com/
- Create a new public git  hub repo
## Step 2: Create a New Repo
## Step 3: Download and Install Git
 - Download Git from https://git-scm.com/download/
 - Install it on your local machine or laptop
## Step 4: Git Configuration
- open the git bash and set up the user name using
  
  `git config --global user.name "your user name"`
- Set up user email
  
  `git config --global user.email "email_address"`
- Check the details

  `git config --list`

## Step 5: Clone the Github repo
- Go to code on github and click on local the select the https and copy the path of your repo. e.g. `https://github.com/example_git-user/eaxmple_github_repo.git`

- Next create a folder in your laptop and go inside it by 

  `cd C:\Users\username\folder`

- Next in the gitbash terminal paste

  `git clone https://github.com/example_git-user/eaxmple_github_repo.git`

- Next go inside the github repo

  `cd example_github_repo/`

- Now check what's inside the repo

  `ls`

- To check all files and folders including hidden item in the repo

  `ls -a`

- Check the git status 

  `git status`

  Shows the current state of your repository, including **tracked** and **untracked files**, **modified files**,**unmodified**,**staged** and branch information

- Create a new text file

  `touch new.txt`

  and add some lines in it.


