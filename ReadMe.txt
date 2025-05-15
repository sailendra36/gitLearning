git -> to check git installed or not

git clone <git repo link> <repoName - optional i.e. if required or already same repo name exists>-> creates a local project based on the link provided

git remove -v -> display the link to the remote repository

git <command> -h -> help with particular command e.g. git clone -h

git add ./git add <file_name> -> add all the files of current dir to staging area

git reset <file_name> -> to unstage a file

git status -> to see staged and unstaged file status

git commit -m "comment" -> commits changes with a comment

git log -> gives logs of commits

git show <commit hash key> -> shows commit details

git show --name-only <commit hash key> -> shows commit details with only changed file name

git reflog -> given info about all commits on all branches in same sequences of changes and checkout done

git branch -> displays overview of all available branches and currently checked out branch

git branch <branchName> -> creates a new branch from master

git checkout <branchName> -> switches/checkouts to other branch

git push -> pushes changes to master branch

git pull -> pulls latest master branch with all commits from other committed branches on different machines

git revert <commit hash key> + :q -> reverts commit with revert commit in logs

git reset --soft <commit hashkey> -> (default if --soft/hard not given) discard all afterwards commits from provided hashkey but keeps the changes - remove commits from history and keeps changes
git reset --hard <commit hashkey> -> discard all afterwards commits from provided hash key but also disregards the changes - remove commits from history and keeps changes
(reset used for clean log i.e. only you are working one the branch but if all team members are working then use revert)
(TC : if you are working on a branch and makes 3 commits but 3rd one is incorrect - do reset)
(TC : if you are working on a branch and makes 3 commits along with other developers also doing their changes but 3rd one is incorrect - do revert so that visible in logs to all)

merge branch <featureBranch> - merges featurebranch into master branch which you are currently in and creates merge commit in logs

Pull Requests
-------------
In FeatureBranch, 
git checkout featureBranch
echo New commit Demo > newCommit.txt
git add .
git commit -m "New Commit"
git push
login to GitHub ->select feature branch from dropdown->new pull request ->create 

Additional daily routine commands 
----------------------------------
git -init -> creates new local repository in a folder
git remote add -> add new remote repository to a project
git diff sourceBranch targetBranch -> difference between 2 branches
git tag -> creates snapshot of the project at certain time(generally branch is tagged before pushing to production for future reference)
git stash -> moves the changes of the project into stash
git stash pop -> retrieves stashed changes and reapply
git rebase -> retrieves all the commits in the master branch and apply the changes to feature branch before your current changes
git clean -> removes untracked files





