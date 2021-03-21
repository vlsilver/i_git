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
    git merge --squash <branch name> //meld all commits of branch name to once commit -> merge to current branch//
    git merge --continue
    git merge --quit
    git merge --abort


Merge branch rebase currentbranch -> branchname:

    git rebase <branch name>
    git rabase --continue
    git rebase --quit
    git rebase --abort

Edit message current commit:

    git commit --amend //quit edit message ":qw" or ":q!"//

Revert current commit:

    git revert HEAD //add new commit delete current commit//

Reset change:

    git reset --hard HEAD

Reset(delete) commit:

    git reset --hard HEAD~ //reset-delete 1 commit from HEAD//
    git reset --hard HEAD~~ //reset-delete 2 commit from HEAD//

Merge commits to current branch:

    git cherry-pick <commitA> <commitB> ...
    git cherrt-pick <commitA>...<commitB>
    git cherry-pick <commitA^...commitB>
    git cheery-pick <branch name> //merge new commit of branch name to current branch//
    git cherry-pick --continue
    git cherry-pick --abort
    git cherry-pick --quit

Meld commits via rebase:

    git rebase -i HEAD~~ //":<key> to quit/save/continue"//git

Edit commit bia rebase:

    git rebase -i HEAD~~
    -> change file.
    git add <file change>
    git commit --amend
    git rebase --continue

Pull all commit of current branch from repository(merge):

    git pull

Fetch all commit of current branch from repositort(create branch FETCH_HEAD handle, not merge):

    git fetch

Push commit from local to repository:

    git push
