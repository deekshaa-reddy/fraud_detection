# fraud_detection
As explained in this video, in the creation of any project, they are three main stages:

Modified: When you change any code in the file.

Staged: When we add the file using ‘git add’, it goes into the staging area.

Committed: When you commit all the changes in the files that were in the staging area. 

We created a file called data_processing.py in our local repository ‘fraud_detection’. Then, we wrote a dummy code in the data processing file and performed the following functions:



#Commands used

git add .

git status

git commit -m “message”

git push -u origin master




Let’s understand these commands in detail:
Git Command
Description
'git add <filename>' or 'git add .'
It is used to add modified files to the staging area. You can add a specific file using the command 'git add <filename>'. If you wish to add all modified and unstaged files present in the workspace to the staging area, you can use the 'git add .' command.
'git status'
This command will display the state of the working directory and the staging area. In other words, it lets you see the changes that have been staged and the changes that have not been added to the staging area.
git commit -m “New commit message”
It gives a new commit message and commits all the files sitting in the staging area.
git push -u origin master or git push 
It is used to upload all the files and changes that were included in the most recent commit to your remote repository on GitHub.
https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html

git reset --hard <commit ID> was used.



Other Important Commands

git log: This command shows you the commit details. It lists out the commits made in the repository in reverse-chronological order, that is, the most recent commits show up first. It shows commits with the following details:
