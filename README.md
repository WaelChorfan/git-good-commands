# the true git init 
rm -rf .git

# the initial  git init 
git init 

# git-good-commands
git update-index --assume-unchanged  <file>
git diff --raw --staged
git log --pretty=oneline
git reset --hard HEAD
git pull --rebase

git branch --set-upstream-to origin/master


 git tag -a v1.0.0 -m "migration api v1.0"

 git push origin v1.0.0



# staging is git add ; to ignote changes to : 
git restore . ( before staging)
git reset ( after staging )



# add repo to folder
git remote add origin https://<urkl>.git

# what to do because no deletion for repo:
https://stackoverflow.com/questions/5363857/delete-all-files-and-history-from-remote-git-repo-without-deleting-repo-itself
git init 
echo "This is the README" > README.md
git add "Readme.md"
git commit -m "Add README.md (initial commit)"
git push origin --mirror



# remove url : 
git remote remove origin


# Create a new branch with current changes 
# First, save your work in progress!
git stash
# Then, one command to create *and* switch to a new branch
git switch -f -c topic/wip HEAD~3






