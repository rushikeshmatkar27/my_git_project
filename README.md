# my_git_project
git assessment

 GIT – Repository & Branching Workflow
Scenario: Your team is starting a new DevOps project. Set up version control for collaboration.

Tasks:

Initialize a Git repository and connect to GitHub.
Create a branch feature/login.
Make changes and commit using meaningful messages.
Merge feature/login into main via pull request or CLI.
Show logs and rollback one commit.

=======================>
=======================>

1-- create the folder--Init--create file--add/commit
17 cd .\my_git_project\
  18 git status
  19 git init
  20 new-item helloword.txt
  21 notepad .\helloword.txt
  22 cat .\helloword.txt...
  23 git status
  24 git add .
  26 git commit -m "first commit"
  27 git status
  
2--create repo on github--copy url---add origin--pull with history--push code to remote main
  29 git branch
  30 git config --list
  31 git remote add origin https://github.com/rushikeshmatkar27/my_git_project
  32 git status
  33 git branch -a
  34 git status
  40 git pull origin main --allow-unrelated-histories
  43 git push origin main
  44 git branch -a

3--create brach--checkout--add file/edit--stage/commit---push to remote dev
  45 git branch dev
  46 git checkout dev
  47 new-item dev.txt
  48 notepad .\dev.txt
  49 cat .\dev.txt
  50 git status
  51 git add .
  52 git commit -m "dev_code_changes"
  53 git status
  54 git push origin dev

4--Merge dev branch with main--browser--repo--pull request--merge

5--git add and reset
  57 git checkout main
  58 git branch -a
  70 notepad .\dev.txt
  71 cat .\dev.txt
  73 git add .
  74 git status
  75 git reset .\dev.txt
  76 git status
 
6--create branch prod--edit code--commit--push--merge code [create pull request(browser)]
  82 git branch -a
  83 git branch prod
  84 git checkout prod
  85 new-item prod.txt
  86 ls
  88 notepad .\prod.txt
  91 git status
  92 git add .\prod.txt
  93 git status
  94 git commit -m "change prod code"
  95 git status
  96 git push origin prod
