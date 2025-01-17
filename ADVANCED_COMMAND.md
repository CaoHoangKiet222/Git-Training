# ADVANCED_COMMAND

## Different

git diff

## Branch

## List Branches

git branch
git branch -a (remote and local)

## Create new branch and switch

git checkout -b <branch_name>

## Switch to new branch

git checkout <branch_name>
git switch <branch_name>

## Delete branch

git branch -d <branch_name>

## Merge

git merge <branch_name> -> (merge <branch_name> to current branch)

## Fix conflicts when merging

## Check where conficts were

git log --merge

## Cancel~Abort current merge

git merge --abort

## Fix merging conflicts

git commit -am "Resloved conflicts"

(git add and git commit to resolve conflicts)

## Tag

## List tags

git tag -l

## Annotated tag

git tag -a <tagname> -m "tag message" <commit_id>

## Lightweight tag

git tag <tagname>

## Delete tag from local

git tag -d <tagname>
git push origin :<tagname>

## Delete tag from remote

git fetch -p
git tag -d <tagname>

## Update tag in local

git tag -f <tagname> <commit_id>
git push -f origin <tagname>

## Push tag to github

git push origin <tagname>
git push --tags -> push all tags

## Stash

## List Stashes

git stash list

## Apply and Drop a stash

git stash pop <stash_name>

## Fetch

git fetch

## Delete local branch from remote

git fetch -p (Before fetching, remove any remote-tracking references that no longer exist on the remote)

## Delete remote branch from local

git branch -D <branch>
git push origin :<branch>

## Git pull with rebase

git pull --rebase

## Synchronize changes back to your fork

git remote add <name> <remote_url>
git pull <name> <branch_name> -p

## Close issue from local

git add <file>
git commit -m "<message>, close #<number>"
git push origin <branch>

## Switch and Create new branch

git fetch --all
git checkout -b <branch_name> <reference>/<branch_name> -> git checkout -b shared-origin origin/shared
