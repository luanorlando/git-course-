# Git Course
Description: Command basic of Git on the Terminal.

 Configuring git 
 ----
### User Namer
$ git config --global user.name "`User name`"

### Email
$ git config --global user.email "`your_email@example.com`"

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

Generating a new SSH key
---

### Add your email
$ ssh-keygen -t rsa -b 4096 -C "`your_email@example.com`"

```sh
Generating public/private rsa key pair.
Enter a file in which to save the key (/Users/you/.ssh/id_rsa): [Press enter] <- 
Enter passphrase (empty for no passphrase): [Type a passphrase] <- Press enter
Enter same passphrase again: [Type passphrase again] <- Press enter
```
### Getting ssh key
$ cd ~/.ssh/
$ ls
$ cat id_rsa.pub or $ more id_rsa.pub

## Adding SSH Key
 - Open your Github, clicked in your profile image and choose "Settings".
 - In "Personal Settings" choose "SSH and GPG Keys".
 - Click in "New SSH key".
 - Add Title.
 - Pass your key in the field "Key".
 exemplo:
 ```sh
 ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQC0lvgtrJBocUGezaLsmKyNS3fF1a8WQrOQwtvuTlhDIsyR3IE1WZNK44M27qKZ5IWO2xAf03pHGtkMcKOimCpoGxkjhStX1owo4b8eWDDRiYrioJm6HD6UAd3OfDQo2IDVwr2c3jU4x/lhMU1vq5TvN/f4IDFhBa30ldurIF9h8/2KMlHW+AqNZm8BQyHw470U551DaggZa23EROQmQDYmvJHYFV3urG4o7NAO309M43j4jLfoShbGDW/YrWuEzvpCzPXp+D63dJ96wHSq3tskEUBKS3a+gTs365Ni6Ui8WelVaTIpokTJELWVRuLd6pX8qawU8PmIKwze3UsUpjuvGBkpvPRq6ORZQ7sydGqtSXZjFYAx68vG158drgdYfM4enE8i/2TKC0ulHBzKH0MzHz+EXvHoNifT7Q8GYJkRydeEaDIZ65iv2edlb5K41c18N2eOFGkEpQdpo1RPYUanZLC1o22vXHGuIUaeMEbyBldmjJCbat4Ttbyql8ebzin9f3k1in2vdmbgSh1E13Vpttn4kRgur3SEjZsVWSPSKIHvpvQfeeqAMtFFtGvFQ== orlandoluan@hotmail.com
 ```

 Creating a new repository
---
 - Open your github page.
 - Click in "New Repository".
 - Enter the name of your repository.
 - Enter with description of your repository.
 - Choose "Public" or "Private".
  ```sh
  Public - Visible to all
  Private - Only you and your guests
  ```
  -  Click in "Create repository".
  
 Adding files to the repository
  ---
  ### Pointing the origin
 $ git remote add origin https://github.com/luanorlando/git-course-.git `<- This url, you will find in the page of your repository`
 
 ### Show repositorys registered
 $ git remote
 
 ### For more details
 $ git remote -v
 
 ### Send to the repository
 $ git push -u origin master
 
 Clone a repository
---
### Command Clone
$ git clone git@github.com:luanorlando/git-course-.git //Enter with a new name `<- address SSH`
$ git clone https://github.com/luanorlando/git-course-.git `<- address HTTPS`

Fork
---
 - Choose a repository
 - In the page this repository, click in fork
 
Branch
 ---
 ### Creating a new branch
 $ git checkout -b  `branch name`
 
 ### Show exiting branch and current branch
 $ git branch
 
 ### Choosing branch
 $ git checkout `'branch name'`
 
 ### Delete branch
 $ git branch -D `branch name`
  
Merge
---
```sn
 - if you create a new branch and add a file, you can do a merge 
```
$ git merge `name of other branch`
$ git commit -m "`message`"

Rebase
---
$ git rebase `name of other branch`

Git Ignore
---
### Ignore all Extension
*.`extension name`

### ignore only file
`File name`

Creating shortcut
---
- Ex: git status
$ git config --global alias.`shortcut name` status
- Now you don't need write git status, only git `shortcut name` <- I will use only the letter `S`

Making their versions with tag
---
### Add tag
$ git tag -a 1.0.0 -m "`Write your message`"
$ git push origin master --tags

### Delete Tag
$ git tag -d `pass the tag`
$ git push origin : `pass the tag`

Revert
---
$ git revert `rash of commit`
$ git show `rash of commit` 

 
Git Hub
---
[Luan orlando](https://github.com/luanorlando)
