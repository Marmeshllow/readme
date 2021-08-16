#GITHELPER
##BASIC
* git init
* git add * or <file_name> or mask
* git rm <file_name> or <folder_name/>
    * -f  *hard delete* 
    * --cached   *safe delete*
* git clone <url>
* git remote -v   *check bound rep*
* git remote add <short_name> <url>   *connect to github rep*
* git commit -a -m "message"  
    * -p
    * -num   *count elm*
    * git commit --amend 
* git status
* git log
    * git log --oneline --graph
    * git log -- <file_name>
* git revert <commit_id>
* git push -u origin master
* git checkout -- <file_name> *restore last commit status for file*


###BRANCH
* git branch <branch_name>
    * git branch  *show all branch*
    * -d   *delete **LOCAL** branch*
* git push --delete origin <branch_name>   *delete **GITHUB** branch! After this need delete local branch*
* git checkout <branch_name>   *change current branch*
* git merge --no-ff <branch_name>
  
###TAG
* git tag -a <tag_name> -m "version 1.0"   *<commit_id> to connect with another commit*
* git tag (show tags)
* git show <tag_name>
* git push --tag    *push tags to github*
* git push --delete origin <tag_name>   *delete **GITHUB** tag! After this need delete local tag*
* git tag -d <tag_name>    *del **LOCAL** tag*
    


