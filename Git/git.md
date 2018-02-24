# Git Tutorial
Create a repository on Github

## Config Git
* git config --global user.name "<my_name>"
* git config --global user.email "<my_email>"
* git config --global core.editor "gedit"

## Git Status
* git status

## Make a project
* mkdir <project_name>
* cd <project_name>
* git init
* create <file or folder>

## Commit a file or folder
* git add <file_or_folder>
* git commit -m "<comment>"

## Delete a file or folder
* git rm <file_or_folder>
* git commit -m "<comment>"

## Create a new branch
* git checkout -b <branch_name>

## Change to a existing branch or master
* git checkout <branch_name>

## Remove a brach
* git branch -d <branch_name>

## Git remote 
* git remote

## Link with Github
* git remote add <remote_name> <github_repository_address>

## Push change to branch (or github)
* git push origin <banch>

## Pull from branch (or github)
* git pull
