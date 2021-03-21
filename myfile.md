# Learn Git Bash with niBVL
## Getting Started
Create file:

    mkdir <file name>

Iniial git: 

    git init

Check change git :

    git status

Add change:

    git add <file name> 
    git add .

Commit:

    git commit -m "<message>"

Create branch:

    git branch <branch name>

Switch branch:

    git checkout <branch name>

Create and switch branch:

    git checkout -b <branch name>

Delete branch:

    git branch -d <branch name>
    git branch -D <branch name>

Merge branch branchname -> current branch:

    git merge <branch name>
    git mere --squash <branch name> //meld all commit of branch name to once commit -> merge current branch//
    git merge --continue 
    git merge --quit
    git merge --abort


Merge branch rebase currentbranch -> branchname:

    git rebase <branch name>
    git rabase --continue
    git rebase --quit
    git merge --abort

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

Edit commit via rebase:

    git rebase -i HEAD~~
    -> change file.
    git add <file change>
    git commit --amend
    git rebase --continue

Stash the changes in a dirty working directory away and clear current branch changes.

    git stash 
    git stash save
    git stash apply [commit] //merge but not delete this commit //
    git stash pop  [commit] //merge and delete this commit//
    git stash list //show all commits of stash//
    git stash show [-p] //show changes desciption of commit//
    git stash branch <branch name> [commit]//create new branch with changes of commit //
    git stash drop [commit] //delete commit in stash//
    git stash clear //delete all commit in stash//

Show changes:

    git diff //show changes not add.//
    git diff --cahed //show changes had add. but not commit//

Pull:

    git pull //get all commit from repository of branch current -> merge it to local //

Fetch:

    git fetch //get all commit from repository of branch current to local//

Push:

    git push //push commit fron local to repository//