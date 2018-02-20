# gitlearning
Learning the basics of GIT

```
$ git init
Reinitialized existing Git repository in D:/Sunil_Kumar/GIT/gitlearning/.git/
```

```
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean
```
## Creating the folder structure in command prompt 
Src
	Classes
		SampleFile.cls (file)
	Pages
		SamplePage (file)

##Various commands used in git
```
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        Src/

nothing added to commit but untracked files present (use "git add" to track)

$ git add Src/

$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   Src/Classes/sampleFile.cls
        new file:   Src/Pages/SamplePage.txt

$ git commit -m "Adding new Files and Folder structure"
[master fe10bd4] Adding new Files and Folder structure
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Src/Classes/sampleFile.cls
 create mode 100644 Src/Pages/SamplePage.txt
```
 
* **To add scripts with the extension .txt**
git add '*.txt'

$ git log
commit 28c36b0c233992d6a0d59550bd8fe62c3ccbf586
Author: Sunil Kumar <sunil.kumar@metacube.com>
Date:   Tue Feb 20 12:33:53 2018 +0530

    Adding new Files and Folder structure

commit d71ebc050ab1fa0bfc2a077ce4d1399bc2989ae7
Author: sunilkhuwal <sunil.khuwal@gmail.com>
Date:   Tue Feb 20 11:59:25 2018 +0530

    Initial commit

* **To track the remote branch**
```
git remote add origin https://github.com/sunilkhuwal/gitlearning.git
```

* **To push the Content to remote master**
```
git push -u origin master
```
* **To pull from origin master**
git pull origin master

* **To view the diff of staged files**
git diff --staged

* **To reset the staged files**
git reset directory/filename.txt

* **To get rid of all the changes since the last commit for file**
git checkout -- directory/filename.txt

* **To create a branch**
git branch branchName

* **To view all the branches**
git branch

* **To switch to a branch**
git checkout branchName

* **To merge the changes of branch1(to merge with current branch) to current branch**
git merge branch1

* **To delete a branch**
git branch -d branchName

