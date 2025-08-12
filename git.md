# Git

#### Git config

    - git config --global user.name [userName]
    - git config --global user.email [emailId]

clone Clone a repository into a new directory
init Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
add Add file contents to the index
mv Move or rename a file, a directory, or a symlink
restore Restore working tree files
rm Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
bisect Use binary search to find the commit that introduced a bug
diff Show changes between commits, commit and working tree, etc
grep Print lines matching a pattern
log Show commit logs
show Show various types of objects
status Show the working tree status

grow, mark and tweak your common history
branch List, create, or delete branches
commit Record changes to the repository
merge Join two or more development histories together
rebase Reapply commits on top of another base tip
reset Reset current HEAD to the specified state
switch Switch branches
tag Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
fetch Download objects and refs from another repository
pull Fetch from and integrate with another repository or a local branch
push Update remote refs along with associated objects

#### Command to clone repository from github to local machine

    - git clone https://github.com/visheshparab/gitHubDemoWindows.git

#### check status

    - git status

#### Add specific file which are modified or created new

    - git add filename

#### Add all files which are modified and created new

    - git add .
    - git add -A

#### save all files and changes on git

    - git commit -m 'message'
      Example: git commit -m '10 new command added in readme.md file, and created new file index.html'

#### push code from local machine to git hub repository

    - git push origin main

#### initializing git in Empty project/repository

    - git init

    - git remote add origin <-link->

#### To verify remote

    - git remote -v

#### To check branch

    - git branch

#### To rename branch

    - git branch -M main

#### To navigate

    - git checkout <-branch_name->

#### To create new branch

    - git checkout -b <-new branch_name->

#### To delete branch

    - git branch -d <-branch_name->

#### List userName and emailId of git

    - git config --list

#### Imagine you’re working on a feature, but an urgent bug fix needs attention. Rather than committing half-done work, you can stash your changes, switch to the bug-fix branch, and return to your feature later without any clutter.

    - git stash
    - git stash apply

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

#### List all branches

    - git branch

#### Create new branch

    - git branch [brachName]

#### Switch to branch

    - git checkout [branchName]

#### Merge changes in master branch (current in master branch)

    - git merge [newFeatureBranchName]

### Local repository to github

    - git remote add origin https://github.com/visheshparab/forkify.git
    - git push origin master
    - git push origin [anotherBranchName] (if you also want to push other branches)

usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
[--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
[-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
[--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
[--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
<command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
clone Clone a repository into a new directory
init Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
add Add file contents to the index
mv Move or rename a file, a directory, or a symlink
restore Restore working tree files
rm Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
bisect Use binary search to find the commit that introduced a bug
diff Show changes between commits, commit and working tree, etc
grep Print lines matching a pattern
log Show commit logs
show Show various types of objects
status Show the working tree status

grow, mark and tweak your common history
branch List, create, or delete branches
commit Record changes to the repository
merge Join two or more development histories together
rebase Reapply commits on top of another base tip
reset Reset current HEAD to the specified state
switch Switch branches
tag Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
fetch Download objects and refs from another repository
pull Fetch from and integrate with another repository or a local branch
push Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

#### check what changes made in file

    - git diff [filename]

#### roleback file to the last saved point or last commit

    - git checkout [filename]

#### revert last git command, to remove all files in staging area

    - git rm cached -r
