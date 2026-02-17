What is the diff b/w branch and tag?
Branch
—-------
Mutable
Creating while development going on
Creating the branches from another branches also.
Git branch [list the branches]
Git branch <name>   [to create a branch]
Git push aliasName Branchname
Git push aliasName --all
Git branch -d branchname


Tag
—-
Immutable
Creating after production deployment
Creating  a tag mainly from master branch
Git tag [List the tags]
Git tag tagName [create a tag]
Git push alias tagName
Git push aliasName --tags
Git tag -d tagname

Step 1: git tag
Step 2: git tag Airtel_V1.0.0[major, minor, patch] —-> create it from master.
Step 3: git tag
Step 4: git push airtel Airtel_V1.0.0

NOTE: tag files always showing in zip and tar


IQ: How to create a tag in remote repository?

Goto tag→create release —> create a tag —-> ……..


Git stash
—---------

When we are working on one task on dev branch, Immediately we got an issue in prod(master), we need to switch.

Step 1: take the working area backup of dev.
     
            git stash save “login feature”
Step 2: see the list of backup.
 
            Git stash list  → stash@{0}, stash@{1} —--

Step 3: go to master branch and finish the work and come back.

Step 3: use the backup to get the data.
      Git stash apply stash@{1}






IQ: In my local repo , size is increasing , How to proceed to reduce that?

Ans: Need to delete all stash files which are not using.
  
Git stash drop —-> by default recent will be deleted.
Git stash drop stash@{5} —> specific one deletion.

NOTE: git stash pop [apply and delete]

git stash clear  —> delete all the stashes at once





How to restore the working area changes?

step 1: wrongly updated file in working area.

step 2: git restore <fileName>
