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

### pull
_used to fetch and download content from a remote repo and immediately update the local repo to match that content_
> git pull origin main

### Init
_used to create a new git repo_<br>

	git init
	git remote add origin <- link ->
	git remote -v (to verify remote)
	git branch    (to check branch)
	git branch -M main (to remote branch)
	git push origin main
	git push -u origin main (from now on we can use git push itself as we have used set upstream function)

### Branch

	git branch		(to check branch)
	git branch -M main		(to rename branch)
	git checkout <-branch name->	(to navigate)
	git checkout -b <-new branch name->		(to create new branch)
	git branch -d <-branch name->		(to delete branch)


### Merge

	git diff <-branch name-> 	(to compare commits, branches, files & more)
	git merge <-branch name->	(to merge 2 branches)


### Undoing changes

	case 1 :  staged changes

		git reset <-file name->
		git reset
	
	case 2 : commited changes (for one commit)

		git reset HEAD~1
	
	case 3 : commited changes (for many commits)

		git reset <-commit hash->
		git reset --hard <-commit hash->

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

### Fork

	Its a new repository that shares code and visibility settings with the original "upstream" repository
	
	> Rough copy