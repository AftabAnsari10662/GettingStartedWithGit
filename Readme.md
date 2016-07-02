##Create a new repository on the command line

* `echo "# Getting Started with Git" >> README.md`
* `git init`
* `git add README.md`
* `git commit -m "first commit"`
* `git remote add origin https://github.com/aftab10662/GettingStartedWithGit.git`
* `git push -u origin master`

##Or push an existing repository from the command line
* `git remote add origin https://github.com/aftab10662/GettingStartedWithGit.git`
* `git push -u origin master`

User Level Configuration
~/.gitconfig
cat ~/.gitconfig
git config --global user.name = "Aftab Ansari"
git config --global user.email = "AftabAnsari10662@gmail.com"
git config --global --list
git config --global help.autocorrect 1
git config --global code.editor vim
git config --global color.ui auto
git config --global core.autocrlf true
--------------------------------------------------------------------------------------------

Repository Level Configuration

git config
stored in .git/config in each Repository.
git config user.name "Aftab"
git config --list
git config --unset core.autocrlf 
----------------------------------------------------------------------------------------------

fetching from a remote
git remote -v
git remote add origin https://github.com/aftab10662/LearningGit.git
git remote rm origin
git fetch 
git merge origin/master

--------------------------------------------------------------------------------------------------
Pulling from a Remote

git branch -r
	git fetch 
	git merge origin master
	
	git pull- if does not work
	git pull --set-upstream master origin/master
	git fetch 

---------------------------------------------------------------------------------------------------
Pushing to a remote

echo "Modify file">>Readme.txt
git commit -am "Pusing to remote"
git push


---------------------------------------------------------------------------------------------------
Creating and Verifying tag

 1. Create tag without message
     git tag v1.0-beta1.0
	 
 2. Create tag with message using -a option .Where a means annotation

    git tag -a v1.0-beta1.1 
	git tag -m "Beta Release" beta-1.0
	
3. View all tags
    git tag
---------------------------------------------------------------------------------------------------
Pushing tags to a remote
 git push --tags

---------------------------------------------------------------------------------------------------
Creating local branches

git branch new-feature
git checkout new-feature
git branch


--------------------------------------------------------------------------------------------------
Renaming and deleting branches
git branch -m fix1 bug1234

git branch -d bug1234
git branch -D bug1234

git checkout -b feature2 = Create branch and do checkout also.

---------------------------------------------------------------------------------------------
##Recovring deleted commits
* `git reflog`
* `git branch fix1 bbf9382`
* `git checkout fix1`
* `git show head`

-----------------------------------------------------------------------------
##Rebasing 

* `git branch extra-feaures beta-1.0`
* `git "Rebasing">>HelloGit.txt`
* `git Commit -am "Rebasing Git "`
* `git rebase master`
* `git checkout master`
* `git merge extra-feaures`
* `git push`


----------------------------------------------------------------------------
Modify the commit.

git add greeter.txt
git commit --amend -m "new commit message"


---------------------------------------------------------------------------
git show HEAD = Show last commit
git show HEAD~10 = 


git commit -am "message"

git branch V1.0_Beta-Branch
git branch - View all local branches.
git branch -r -- View all Remote branches.
git branch --all
git checkout V1.0_Beta-Branch
git push origin V1.0_Beta-Branch
git branch -r

git tag V1.0
git tag -a V1.0_With_Message
git tag- View All Tag
git push --tag

git pull origin master

git remote rm origin
git remote
git remote -v - View All associated Remote Repository
git remote add origin git@github.com:aftab10662/LearningGit.git
git remote add origin https://github.com/aftab10662/Learning.git

git branch --set-upstream master origin/master.




git fetch- fetch from Remote Repo.
git fetch origin -- fetch if you have multiple remote.
git push - push to remote Repo.
git push origin - if you have multiple remote.

git pull origin master- pull form remote origin branch.

git push --tag.

git fetch origin;git merge origin/master; = git pull origin;


git log --graph --online
git log --graph --oneline --all --decorate
git config --global alias.gla "log --graph --oneline --all --decorate"
 
 
 Using Alias
 
 git config alias.st status
 git config --global alias.co checkout
 git config --global alias.cma "commit --all -m"

git show-ref --heads
git branch -d V2.0_Beta




Sync Local forked Repo with MAster Repo
>git remote -v
git aspnet fetch
git checkout master
git merge aspnet/master
git rebase aspnet/master
git push origin master

git commit -am "Merge Conflicts Resolvedx`"

git branch ng2-fix 77b1b35


