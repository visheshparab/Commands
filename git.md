# Git

#### initializing git in Empty project/repository

    - git init

#### Git config

    - git config --global user.name [userName]
    - git config --global user.email [emailId]

#### Command to clone repository from github to local machine

    - git clone [https://github.com/visheshparab/gitHubDemoWindows.git]

#### check status

    - git status

#### Add specific file in staging

    - git add filename

#### Add all files in staging

    - git add .
    - git add -A

#### save all files to local repository

    - git commit -m 'message'
      Example: git commit -m '10 new command added in readme.md file, and created new file index.html'

#### push code from local machine to git hub repository

    - git push origin main
    - git push -u origin main (After this command, we can only run git push)

#### Add local repository files to github repository

    - git remote add origin <-link->

#### To verify remote

    - git remote -v

#### To check branch

    - git branch

#### To rename branch

    - git branch -M main

#### To delete branch

    - git branch -d <-branch_name->

#### List userName and emailId of git

    - git config --list (run this command in root directory: cd)

#### Move changes temporarily to shelf so that you can switch branch without staging or commiting

    - git stash

#### Bring back stash changes

    - git stash pop

#### List all stash

    - git stash list

#### Imagine you’re working on a feature, but an urgent bug fix needs attention. Rather than committing half-done work, you can stash your changes, switch to the bug-fix branch, and return to your feature later without any clutter.

    - git stash
    - git stash apply [stashCode]

#### git reflog can save you. It keeps track of all changes to the tip of branches, helping you recover lost commits.

    - git reflog

#### Debugging can be frustrating, especially when you’re unsure when a bug was introduced. git bisect performs a binary search through your commit history to find the exact commit where things went wrong.

    - git bisect start
    - git bisect good <last known good commit>
    - git bisect bad <bad commit>

#### Sometimes you don’t want to merge an entire branch but still need to include specific commits. git cherry-pick allows you to take specific commits from one branch and apply them to another. You’re working on a new feature, and your teammate fixes a bug on a different branch. Instead of merging the entire branch, you can cherry-pick that one bug fix and apply it to your working branch.

    - git cherry-pick <commit-hash>

#### git reset — — hard is a powerful but dangerous command. It resets your working directory to a specific commit, discarding any changes that have not been committed. Say your project is in a broken state and you want to start fresh from a previous commit. git reset — — hard allows you to revert all changes back to a stable commit. Just be cautious, as it removes uncommitted changes.

    - git reset --hard <commit-hash>

#### Need to know who made the last change to a particular line in a file? git blame shows you a detailed history of who changed what, and when. If you’re trying to understand why a piece of code behaves in a certain way, git blame helps you trace back to the original author. This is especially useful for debugging or code reviews.

    - git blame <file>

#### Over time, your project can accumulate many untracked files, like build artifacts or logs. git clean helps you clean up by removing these files from your working directory. After multiple builds or experiments, your project might have leftover files that aren’t tracked by Git. git clean keeps your workspace tidy by removing unnecessary files and directories.

    - git clean -f
    - git clean -fd

#### Ever wanted to see a summary of who contributed to a project? git shortlog groups commit by author, making it easy to see who has been working on what. In open-source projects or large teams, git shortlog provides a quick overview of each developer’s contributions. It’s also handy for generating contribution stats for reports or presentations.

    - git shortlog -s -n

#### Jump to previous commit

    - git reset --hard HEAD

#### Jump to specific commit

    - git reset --hard [commitId]

#### Log of all commits

    - git log
    - git log --oneline (logs all commits in one line)

#### List all branches

    - git branch

#### Create new branch

    - git branch [brachName]

#### To rename branch

    - git branch -m main (first switch to branch you want to rename, then run this command)

#### To switch branch

    - git checkout [branchName]
    - git switch [branchName]

#### Create new branch and switch to created branch

    - git checkout -b [branchName]
    - git switch -c [branchName]

#### To delete branch

    - git branch -d [branchName]

#### Merge changes in master branch (current in master branch)

    - git merge [newFeatureBranchName]

#### check what changes made in file

    - git diff [filename]
    - git diff --staged  (displays changes made by file which are currently in staging)
    - git diff [commitId1] [commitId2]  (displays changes with specific commit)
    - git diff [commitId1]..[commitId2]

#### roleback file to the last saved point or last commit

    - git checkout [filename]
    - git checkout [commitId]  (roleback to specific commit checkpoint)
    - git checkout HEAD~2      (roleback 2 commit back)

#### revert last git command, to remove all files in staging area

    - git rm cached -r

#### Set code editor to write commit message (below command is for vscode editor)

    - git config --global core.editor "code --wait"

#### Get details of username, email and other configuration on git

    - cat .gitconfig
