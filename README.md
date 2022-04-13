Day1:
1.create github account 
2.create public repository 
#git clone repo url
#cd reponame
#touch file1.txt file2.txt (touch --> creating files)
#vi filename (insert I --> data given -->Esc--> Shift+: --> wq!)
#mkdir folder1 folder2  (mkdir-->creating directory)
#git add *
#git commit -m “ message”
#git log 
#git config —global user.email “sidd.nar@gmail.com”  ( one time activity)
#git config — global user.name “username of git hub”
#git push origin main or master 

Day2:
# git pull repourl( updates comes)( commit message new to give in vi editor)
# git fetch ( updates comes into local but it directly it won't reflect, once merge command applied then it will reflect into local)
# git merge 
# git branch name (creating new branch)
# git checkout branch name (switch to branch)
# git checkout -b branch name( create and switch branch)
# git checkout -d branch name( deleting branch name)

STASH: to hide data in branch
Add files in git 
# git add *
# git stash 
# git list
# git stash apply 
# git stash apply stash 
FORK:
# git fork ( copy of our original repository)
COLLABORATOR ACCESS:
git collaborator acces given for developers in GitHub --> settings
PULL REQUEST:
github dashboard--> pull request--> mention source branch & destination branch --> add reviewers-->merge these branches

Day3:
RESET: ( undoing changes)
# touch one.txt two.txt
# git add *
# git commit -m "message"
# git log or git log --oneline
# git reset --hard HEAD~1 or commitID
#  git reset --mixed HEAD~1 or COMMITID
# git status
# touch three.txt 
# git add *
# git reset three.txt  (no need to mention soft)
REVERT: ( commit message change & new commit)
# touch one.txt two.txt
# git add *
# git commit -m "message"
# git log or git log --oneline
# git revert commitID  (update message)
# git log --oneline
MERGE:( two different branched, every merge commit id generate )
# git branch DEV
# git checkout DEV
# touch d1 d2 d3
# git add *
# git commit -m "devfiles"
#git checkout main
# ls
# git merge DEV
# ls or git log --oneline
REBASE: (merging two different branches it wont generate commit id for every rebase)
# git branch TEST
# git checkout TEST
# touch d1 d2 d3
# git add *
# git commit -m "devfiles"
#git checkout main
# ls
# git merge TEST
# ls or git log --oneline

Day4:
CHERRY-PICK: ( merge single commitid)
# git branch TEST
# git checkout TEST
# touch t1 t2 t3
# git add *
# git commit -m "testfiles"
# git log --oneline
#git checkout main
# git cherry-pick COMMITID

#git commit --amend -m  (modify latest commit message)
#git blame filename  ( used to show what revision and author last modified each line of a file. It's like checking the history of the development of a file).
#git tag (show versions)
