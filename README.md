The Basic course on GIT was completed:

Git is a version control system widely used by developers to track changes to a project's source code. Here are some basic Git commands:

git init

Initializes a new Git repository. Executed once when creating a new project.
bash
Copy code
git init
git clone

Clones an existing Git repository. Used to create a local copy of a remote repository.
bash
Copy code
git clone <repository_URL>
git add

Adds changed or new files to the index, preparing them for commit.
bash
Copy code
git add <filename>
git commit

Commits the changes added to the index and creates a new version (commit).
bash
Copy code
git commit -m "Commit description"
git status

Shows the status of the working directory: changed files, files in the index, etc.
bash
Copy code
git status
git pull

Updates the local repository with data from the remote repository.
bash
Copy code
git pull
git push

Pushes changes from a local repository to a remote repository.
bash
Copy code
git push
git branch

Shows a list of local branches and the current active branch.
bash
Copy code
git branch
git checkout

Switches between branches.
bash
Copy code
git checkout <branch name>
git merge

Merges changes from one branch to another.
bash
Copy code
git merge <branch name>
git log

Shows commit history.
bash
Copy code
git log
git remote

Shows a list of remote repositories.
bash
Copy code
git remote -v


GIT - Distributed Version Control System
  Global Information Tracker

git --version - whether git is installed


git config --local user.name "Vladimir Yankers"

First!!!!!!!! Let's create user data!

git config --global user.name "Vladimir"
git config --global user.email Vovarojko@gmail.com
git config --list - check git settings
q - quit - leave

Linux commands:
Vova@Yankers MINGW64 ~/Desktop
$ mkdir my-project

Vova@Yankers MINGW64 ~/Desktop
$cd my-project/

Vova@Yankers MINGW64 ~/Desktop/my-project
$pwd
/c/Users/Vova/Desktop/my-project

Vova@Yankers MINGW64 ~/Desktop/my-project
$ls

Vova@Yankers MINGW64 ~/Desktop/my-project
$ echo "Some text" > file.txt

Vova@Yankers MINGW64 ~/Desktop/my-project
$ls
file.txt

Vova@Yankers MINGW64 ~/Desktop/my-project
$ cat file.txt
Some text

Vova@Yankers MINGW64 ~/Desktop/my-project
$rm file.txt

Vova@Yankers MINGW64 ~/Desktop/my-project
$ls

Vova@Yankers MINGW64 ~/Desktop/my-project



Create a repository:

git init - in the folder we want to create - a .git folder is created - but it can be hidden
ls -la - Mac
ls -Forse - show hidden files and folders (Windwows)
1) Current directory

Create a git init repository (by default we are in the Master branch)
git branch -m main - rename web development

2) When the files are created and Git monitor their status

Git status (staging area - index)



0) git add - adding to stage area (index)
1) Git add -A - all files in the repository, add for tracking
2) git add main.*css

git commit status

git commit -a -m "ffirst commit" ( -m specify a message, if not specified, then a message will be displayed about what to specify!)
git commit -m "message"

git log - look at all commits - SHA1 and indicates which commit we are on!!!!!!!!!!!!!
git checkout <commit hash> - SHA1 move by commit (head - move by commit)
git checkout <branch name> - branch transition

git add file-text.txt - one file in staging area (index)
git add . - all files in index

git commit -m "First-commit" created with sha1 9ad8bc8

commit 90432a87849012ae32707bf702427c517ef493fa (HEAD -> master) 90 - folder name, the rest is the name of the text file
Author: Vova Yankers <vovarojko@gmail.com>
Date: Fri Nov 11 16:59:23 2022 +0200

Shuffle by SHA1:
git cat-file -t 90432a - commit
git cat-file -p 90432a - who created the commit and who is the author (contents):
$ git cat-file -p f7b9c
040000 tree 74b6896366125aad77337f7f7c251bd3ea0c9ef5 3 areas git
100644 blob cbef9cf735761ebc2581fe215d89b314aab2a2e0 GIT.txt
040000 tree 32ef472c6b7a64d9f397090249af49dc12c896e2 first-subfolder
100644 blob 0d5c361af63517ec1ef03f7bf247c95e03411420 index.html
100644 blob e69de29bb2d1d6434b8b29ae775ad8c2e48c5391 script.js
040000 tree 71234083c8cc74e9af46b881fa501869e8f53519 second-subfolder



     Push to the cloud!!!
1)git remote add origin https://github.com/Gunplay/project.git

2)git branch -M main

3) git push -u origin main - -u push to this repository by default

Cloning to another computer!!
PS D:\Learn HTML, CSS\03 Module 3. Necessary technologies for a web developer and advanced practice> cd work
PS D:\Learn HTML, CSS\03 Module 3. Necessary technologies for a web developer and advanced practice\work> ls
PS D:\Learn HTML, CSS\03 Module 3. Necessary technologies for a web developer and advanced practice\work> git clone https://github.com/Gunplay/project.git project_2

Git pull - for data synchronization!!!!!! When we work as a team!
