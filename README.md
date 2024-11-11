# github-learnings

## Git
_Version control system_
	
 **Purpose**
	
 - track the history of the code
 - collaborate

## Github
_Website that allows developers to store and manage their code using git._

 **Purpose**
	
 - Can upload your own projects
 - Copy others repositories and make changes to it
	
## Configuring Git

- git config --global user.name "My Name"
- git config --global user.email "someone@email.com"
- git config --list

## Git Commands

### clone
_cloning a repository on our local machine_
<br>
> git clone <-some link ->

### status
_display state of the code_
<br>
> git status

### add
_adds new or changed files in your working directory to the Get staging area_
> git add <- file name ->

### commit
_it is the record of change_
> git commit -m "some message"

### push
_to upload local repo content to remote repo_
> git push origin main

### Init
<br>_used to create a new git repo_

> git init
> git remote add origin <- link ->
> git remote -v (to verify remote)
> git branch    (to check branch)
> git branch -M main (to remote branch)
> git push origin main
> git push -u origin main (from now on we can use git push itself as we have used set upstream function)


### types of messages for file on IDEs

**untracked**
<br>_new files that git dosen't yet track_

**modified**
<br>changed

**staged**
<br>_file is added & ready to be committed_

**unmodified**
<br>_unchanged_

## Workflow
Github repo > Clone > Changes > Add > Commit > Push