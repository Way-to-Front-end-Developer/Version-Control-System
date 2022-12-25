# Git

https://git-scm.com/  
https://docs.github.com/en/get-started/using-git/about-git  
https://www.w3schools.com/git/default.asp?remote=github

**Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.**     

Developers can review project history to find out:  
Which changes were made?  
Who made the changes?  
When were the changes made?  
Why were changes needed?

Cистемы контроля версий можно разделить на:  
**локальные** (один клиент и локальные копии отдельных файлов)  
**централизованные** (один или более клиентов, единственный сервер, содержащий все версии файлов проекта и каждый клиент может получить определенную версию этого файла)  
**распределенные** (один или более клиентов, единственный сервер, содержащий все версии файлов проекта и каждый клиент может получить определенную версию целого проекта)

# Basic

Git is a version control system, helps you keep track of code changes, used to collaborate on code.

**Git - это система контроля версий.** это хранилище базы данных для истории разработки проекта который содержит все версии его файлов как текущие так и старые уже не актуальны, мы добавляем в него начальной версии наших файлов и потом когда мы что-то редактировали то мы добавляем в git обновленную версию и git тоже себя записывает и что самое замечательное мы всегда можем залезть в это хранилище посмотреть что там лежит и восстановить предыдущие версии файлов особенно здорово то что гид может не только хранить версии но и позволяет обмениваться ими между разработчиками в отличие от простого копирования в git есть встроенные средства обнаружения конфликтов и интеграции изменений так что есть два разработчика вдруг даже поменяли один и тот же файл то они смогут это легко увидеть и объединить свои изменения а в простых случаях гид даже делает это автоматически

**гид называют распределенные системы контроля** версий потому что мне не требуется центральный сервер у каждого
разработчика стоит локальная копия гид которая хранит историю разработки проекта когда он что то сделал он в
первую очередь записывает это к себе на компьютер свой git а потом если захочет может связано с коллегами
отправить им свои измерения получить их однако в реальных проектах центральный сервер как правило делают он служит для
удобства на него все разработчики отправляют свои изменения и с него могут скачать то что сделали их коллеги в
данном случае сервер не выполняет никакой умные работы это всего лишь центральный пункт обмена данными все основные операции по
прежнему выполняются локально в качестве гид сервера часто используют гитхаба это интернет сервис который находится по этому адресу и он позволяет
не только хранить проект ну и предлагать обсуждать изменения в коде это очень удобно и наконец последняя но от этого
не менее важная git это надежная система то есть если у нас файлы лежат просто на диске мало ли что повреждение жесткого диска или сбой
памяти если у нас файлов много мы можем даже не сразу это заметить в то время как git не просто хранит версии файлов
он для всего вычисляет контрольную сумму и если хоть где-нибудь данные будут повреждены то мы обязательно это обнаружен ну а так
как git это распределенная система у каждого работника есть своя копии история проекта то автоматически получается такой большой большой
надёжный backup если файлы повредились у меня то я легко смогу восстановить их у коллеги это еще одна причина по которой весь код проекта лучше хранить гит гит
это надежно и очень удобно 


**git vs github**
https://www.geeksforgeeks.org/difference-between-git-and-github/****


Main commands:

`cd`  - changes the current working directory.
`mkdir` - makes a new directory.  
`ls`  - command that lists the file contents of a directory.
`dir` - in Command Prompt to list all of the files and folders in the current directory.
`clear` - clear the terminal.  
`rm` command can be used to remove individual files or a collection of files

Git commands:

`git init` - initialized empty Git repository in ...  

**Note**: Git now knows that it should watch the folder you initiated it on.  
Git creates a hidden folder to keep track of changes.

Files in your Git repository folder can be in one of 2 states:  
`Tracked` - files that Git knows about and are added to the repository  
`Untracked` - files that are in your working directory, but not added to the repository

One of the core functions of Git is the concepts of the `Staging Environment`, and the `Commit`.

`git --version` - check version of git  
`git pull` - updates the local line of development with updates from its remote counterpart.  
`git fetch` - command downloads commits, files, and refs from a remote repository into your local repo.   
`git rebase` - 

`git pull vs git fetch`  
https://www.geeksforgeeks.org/git-difference-between-git-fetch-and-git-pull/#:~:text=Git%20Fetch%20is%20the%20command,changes%20into%20the%20local%20repository.

`git reset` - command is a complex and versatile tool for undoing changes  
We reset our repository back to the specific commit using git reset commithash (commithash being the first 7 characters of the commit hash we found in the log).

`git revert` - command we use when we want to take a previous commit and add it as a new commit, keeping the log intact.

`git checkout vs git switch`  
https://linuxhandbook.com/git-switch-checkout/#:~:text=Git%20checkout%20is%20the%20old,working%20tree%20without%20switching%20branches.

`git log --oneline` - show all commits

`git command -help` -  See all the available options for the specific command  
`git help --all` -   See all possible commands

`origin` - in Git, `origin` is a shorthand name for the remote repository that a project was originally cloned from. More precisely, it is used instead of that original repository's URL - and thereby makes referencing much easier.

### Branch

In Git, a `branch` is a new/separate version of the main repository.

`git branch <branch>` - creates a new branch

`-D` - flag for delete a branch
