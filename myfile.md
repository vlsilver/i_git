# Learn Git Bash with niBVL
## Getting Started
Create file:

    mkdir <file name>

Iniial git: 

    git init

Check change git :

    git status
    git status -s // show file change and type change //

Add change:

    git add <file name> 
    git add .

Commit:

    git commit -m "<message>"

Show all commit:

    git log
    git log --decorate //show all commits and them tag//

Create branch:

    git branch <branch name>

Show all branch:

    git branch

Switch branch:

    git checkout <branch name>

Create and switch branch:

    git checkout -b <branch name>

Delete branch:

    git branch -d <branch name>
    git branch -D <branch name>

Merge branch branchname -> current branch:

    git merge <branch name>

Merge branch rebase currentbranch -> branchname:

    git rebase <branch name>

Add tag for current commit:

    git tag <tag name>

Show all tab:

    git tag