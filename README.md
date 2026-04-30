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





###file
deves@Devesh MINGW64 ~
$ cd fraud_dectection/
bash: cd: fraud_dectection/: No such file or directory

deves@Devesh MINGW64 ~
$ cd fraud_detection

deves@Devesh MINGW64 ~/fraud_detection
$ echo "# fraud_detection" >> README.md

deves@Devesh MINGW64 ~/fraud_detection
$ ls
README.md

deves@Devesh MINGW64 ~/fraud_detection
$ cat README.md
# fraud_detection

deves@Devesh MINGW64 ~/fraud_detection
$ git init
Initialized empty Git repository in C:/Users/deves/fraud_detection/.git/

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git config user.name deekshaa-reddy

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git config user.email deekshareddy13579@gmail.com

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git config user.name
deekshaa-reddy

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git config user.email
deekshareddy13579@gmail.com

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


deves@Devesh MINGW64 ~/fraud_detection (master)
$ git commit -m "first comment adding readme file"
[master (root-commit) 0b9f024] first comment adding readme file
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git status
On branch master
nothing to commit, working tree clean

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git branch
* master

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git remote add origin https://github.com/deekshaa-reddy/fraud_detection.git

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git push -u origin master
info: please complete authentication in your browser...
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 247 bytes | 82.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/deekshaa-reddy/fraud_detection.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

deves@Devesh MINGW64 ~/fraud_detection (master)
$ ^C



#### Revert and reset### Branching
### check branch and add
deves@Devesh MINGW64 ~/fraud_detection (master)
$ git branch
* master

deves@Devesh MINGW64 ~/fraud_detection (master)
$ git checkout -b model
Switched to a new branch 'model'

deves@Devesh MINGW64 ~/fraud_detection (model)
$ git branch
  master
* model

### created a ML file 

deves@Devesh MINGW64 ~/fraud_detection (model)
$ git status
On branch model
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ml_model.py

nothing added to commit but untracked files present (use "git add" to track)

deves@Devesh MINGW64 ~/fraud_detection (model)
$ git add ml_model.py

deves@Devesh MINGW64 ~/fraud_detection (model)
$ git status
On branch model
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   ml_model.py


deves@Devesh MINGW64 ~/fraud_detection (model)
$ git commit -m 'added ml model code'
[model 41214a6] added ml model code
 1 file changed, 1 insertion(+)
 create mode 100644 ml_model.py

deves@Devesh MINGW64 ~/fraud_detection (model)
$ git status
On branch model
nothing to commit, working tree clean

## added to branch
deves@Devesh MINGW64 ~/fraud_detection (model)
$ git push origin model
Enumerating objects: 12, done.

## Commit changes in branch

This is done in guthub . where admin will go through the branch check files changes later accept the push request to commit



