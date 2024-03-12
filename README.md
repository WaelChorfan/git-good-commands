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

#good links
# vs code search (activate regex as well)
To apply logical and (?=.*word1)(?=.*word2)(?=.*word3)
To apply logical or (word1)|(word2)|(word3)

#delay function in apex

    public static void delayInMilliSeconds(Integer ms) {
        Datetime start = System.Now();
        while (System.Now().getTime() < start.getTime() + ms) {
        }
    }

# get rec type id by sobject and field name
   public static Id getRecordTypeId(String sObjectName, String recordTypeName) {
        Id recordTypeId = Schema.getGlobalDescribe().get(sObjectName).getDescribe().getRecordTypeInfosByName().get(recordTypeName).getRecordTypeId();
        return recordTypeId;
    }
# prettier install

npm install --save-dev --save-exact prettier prettier-plugin-apex
 # java path for that
  C:\\open_jdk-11.0.21.9-hotspot
{
  "salesforcedx-vscode-apex.java.home": "C:\\open_jdk-11.0.21.9-hotspot",
  "salesforcedx-vscode-core.retrieve-test-code-coverage": true
}

# pull remote branches 
 git branch -a
 



# apex class run tests 
sf apex run test -n classA, classB , ...
