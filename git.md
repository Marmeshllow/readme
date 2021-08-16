#GITHELPER
##BASIC
* git init
* git add * or <file_name> or mask
* git rm <file_name> or <folder_name/>
    * git rm -f <file_name>  *Полное удаление* 
    * git rm --cached <file_name>   *Удаление из отслеживаемого*
* git clone <url>
* git remote -v   *Просмотр привязанных репозиториев*
* git remote add <short_name> <url>   *Связь с удаленным репозиторием*
* git commit -a -m "message"
    * git commit --amend 
* git status
* git log
    * git log --oneline --graph
    * git log -- <file_name>
    * git log -p *Подробная информация*
    * git log - <num>   *Ограничение на кол-во выводимых комитов*
    * git log --grep <'commit comment'> *Поиск по коментам*
    * git log -S <'string code'>
    * git log --all *По всем весткам*
* git blame --<file_name> [KEKW](https://media.makeameme.org/created/i-dont-know-5c3e1e.jpg)
* git show <commit_ad> or <tag> *--<file_name> Не обязательно*
* git push -u origin master



###BRANCH
* git branch <branch_name>
    * git branch  *Показать ветки*
    * -d   *Удалить **LOCAL** ветку*
* git push --delete origin <branch_name>   *Удалить **GITHUB** ветку! После нужно удалить **LOCAL** ветку*
* git checkout <branch_name>   *Смена ветки*
    * git checkout -b <branch_name> *Создание новой и переход в нее*
* git merge --no-ff <branch_name>
  
###TAG
* git tag -a <tag_name> -m "version 1.0"   *<commit_id> Для присвоения тега др коммиту*
* git tag *Показать теги*
* git show <tag_name>
* git push --tag    *Запушить теги на GITHUB*
* git push --delete origin <tag_name>   *Удалить тег с **GITHUB!** После нужно удалить **LOCAL** тег*
* git tag -d <tag_name>    *Удалить **LOCAL** тег*


###RESTORE
* git checkout <commit_id> *Передвинуть **HEAD***
* git revert <commit_id> *Откат назад и создание нового комита*
* git reset <mode> <commit_id>
    * git reset -hard <commit_id> *Ничего не сохраняет*
    * git reset -soft <commit_id> *Все сохраняет*
    * git reset -mixed <commit_id> *Все отмененные изменения оставляет в рабочей директории*
* git reset <mode> HEAD~<num>  *Откат от позиции HEAD на NUM шагов*

