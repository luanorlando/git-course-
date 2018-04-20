# Git Course
Description: Command basic of Git on the Terminal.

 Configuring git 
 ----
### User Namer
$ git config --global user.name "Luan Orlando"

### Email
$ git config --global user.email "orlandoluan@hotmail.com"

### Editor
$ git config --global core.editor "`Pass name of editor`"

Request values
---
### User name
$ git config user.name

### Email
$ git config user.email

### All
$ git config --list

Starting a repository
----
### Create folder
$ mkdir `name of folder`

### Enter the folder
$ cd `name of folder`

### Starting git
$ git init

### Show content folder
$ ls

### Go back to the previous folder
$ cd ..

First commands
---
### Status
$ git status

### Add file
$ git add Reademe.md

### Add All
$ git add --all

### Commit
$ git commit -m "`Write message of your comments, usually comments on that was done`"

### Add and commit
$ git commit -am "`message`"

```sh
//You can upload the file to the repository
$ git push origin master
```

Viewing logs
---
### Log
$ git log

### Decorate
$ git log --decorate

### All the author's commits 
$ git log --author="`author's name`"

### Authors, number of commits and all commits
$ git shortlog

### Only number of commits and Author's name
$ git shortlog -sn

### Show graph
$ git log --graph

### show rash
$ git show `rash's number`

### show modifications
$ git diff

### show only file name
$ git diff --name-only

Reset files
---
### Return the file before editing
$ git checkout `file name`

### Return the file after it has been added
$ git reset HEAD `file name` //Remove of stage
//After
$ git checkout `file name`

## Return the file after it has been added and commited
### Soft
$ git reset --soft `rash of a previous commit than you wish to delete`
$ git commit -m "`message`"
### Mixed
$ git reset --mixed `rash of a previous commit than you wish to delete`
$ git add --all
$ git commit -m "`message`"
### Hard
$ git reset --hard `rash of a previous commit than you wish to delete`
//Reseted all


`loojhgjhfg`

jjghjgkjgk
---

[hjgjkgjhgjk](http://hgjgjgj)

- jjkhkh
1. ohkhhi

* jghgghj

```sh
APIController
AreaInteresseController
WebServiceController
DisponibilidadeController
HomeController
IdiomaController
LoginController
TemplateController
```



`
