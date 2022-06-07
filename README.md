# COMMANDS

git init <file>
git add .
git commit -m ""
git commit -am "" # can use when file tracked -> (git add <file> && git commit -m "")

git status
git show
git ls-files # show all files tracked

git reset HEAD <file>

# the same as (git restore --staged <file>)

git check-out -- <file>

# the same as (git restore <file>)

git log --oneline --graph --decorate --all
git config --global alias.<name> "<command> except git"

# eg. git config --global alias.hist "log --oneline --graph --decorate --all" -> git hist (to use)

git mv <file> <new_file>(in staging area or in local repository)
git commit -m "move file"

git rm <file> <new_file>(in staging area or in local repository)
git commit -m "remove file"
