# Git

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

6. Command to clone repository from github to local machine

   - git clone https://github.com/visheshparab/gitHubDemoWindows.git

7. check status

   - git status

8. Add specific file which are modified or created new

   - git add filename

9. Add all files which are modified and created new

   - git add .

10. save all files and changes on git

    - git commit -m 'message'
      Example: git commit -m '10 new command added in readme.md file, and created new file index.html'

11. push code from local machine to git hub repository

    - git push origin main

12. initializing git in Empty project/repository

    - git init

    - git remote add origin <-link->

13. To verify remote

    - git remote -v

14. To check branch

    - git branch

15. To rename branch

    - git branch -M main

16. To navigate

    - git checkout <-branch_name->

17. To create new branch

    - git checkout -b <-new branch_name->

18. To delete branch

    - git branch -d <-branch_name->
