# workshop-git

## Outline

* [The Git Parable](http://tom.preston-werner.com/2009/05/19/the-git-parable.html)
* Setup
    *   git help 
    *   git init
    *   git config
    *   git alias
    *   Exercise 1
* [Git Areas](http://ndpsoftware.com/git-cheatsheet.html)
* Saving Changes
    *   git status
    *   git add
    *   git commit [--amend]
    *   git diff [--staged]
    *   git reset HEAD
    *   git checkout [-- filename]
    *   git stash
    *   git revert
    *   Exercise 2
* Reading history
    *   git log
    *   git blame
    *   git reset HEAD~n
    *   git reflog
    *   Exercise 3
* Navigating Repository
    *   Detached HEAD
    *   Branches
        *   git checkout -b
        *   git checkout
        *   git branch
        *   git cherry-pick [--edit]
        *   [Demo](https://learngitbranching.js.org/?NODEMO)
        *   Exercise 4
        *   Exercise 5 - move commit
    * Tags
        *   git tag
        *   git checkout
        *   [Demo](https://learngitbranching.js.org/?NODEMO)
* Remotes
    * git clone
    * git remote
    * git fetch
    * git push
    * git pull
    * git checkout
    * Exercise 6
* Managing Branches
    * git merge
    * git rebase 
    * Merge Vs Rebase
    * Managing Conflicts
        * git mergetool
        * VSCode example
    * Exercise 7
* Workflows
    * All master
    * Feature Branches
    * master, develop and feature branches
    * Pull requests
    * Feature Flags
    * Exercises
* Tools
    * tig
    * SourceTree
    * GitKraken
    * Gitup

### Exercises

#### Exercise 1

Create an empty repository and then config the local repository with a different email than the global one. Assign then a global alias to easily set the email to the local repository.

#### Exercise 2

Create a new file. Add the file to the staging area and then commit it. Change the commit message to a new one. 

Modify the file, stash the modifications. Modify the file again and commit the changes. Apply the stash, without deleting it. 

Modify some files, then delete all modifications.

#### Exercise 3

Modify and commit a file, check it with git log and git blame. Then return to the previous commit. Try to use reflog to recover the lost commit

#### Exercise 4

Create a file and commit it on master. Create a branch and commit one modification, then cherry pick the modification on master. Delete the other branch.

#### Exercise 5

Create a file and commit it on master. Modify the file again and commit it. The last commit is an error, it should be on a branch called "test". Fix the situation.

#### Exercise 6

Fork this repo and clone it. Open various branches and push them. Delete the repo and clone it again, try to go on one of the branches that you pushed.

#### Exercise 7

Create two branches from master, do a bunch of commits on the same file in both branches. Now try get all the code from both branches on master and manage the conflicts. Do that using merge and rebase and think about the differences.