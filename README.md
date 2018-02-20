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

 $ git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

Counting objects: 6, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (6/6), 474 bytes | 0 bytes/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/sunilkhuwal/gitlearning.git
   d71ebc0..fe10bd4  master -> master


To add scripts with the extension .txt
git add '*.txt'

$ git log
commit 28c36b0c233992d6a0d59550bd8fe62c3ccbf586
Author: Sunil Kumar <sunil.kumar@metacube.com>
Date:   Tue Feb 20 12:33:53 2018 +0530

    updating readme file

commit 12dea1e3f502bfb51614f3e488b7d4b678b35e0d
Author: Sunil Kumar <sunil.kumar@metacube.com>
Date:   Tue Feb 20 12:31:53 2018 +0530

    updating readme file

commit fe10bd41c844d029d86d12816ca69d80579c83b2
Author: Sunil Kumar <sunil.kumar@metacube.com>
Date:   Tue Feb 20 12:07:48 2018 +0530

    Adding new Files and Folder structure

commit d71ebc050ab1fa0bfc2a077ce4d1399bc2989ae7
Author: sunilkhuwal <sunil.khuwal@gmail.com>
Date:   Tue Feb 20 11:59:25 2018 +0530

    Initial commit

	**To track the remote branch **
	```
	 git remote add origin https://github.com/sunilkhuwal/gitlearning.git
	```

	 **To push the Content to remote master**
	 ```
	 git push -u origin master
	 ```
	 **To pull from origin master**
	 git pull origin master
	 
	 **To view the diff of staged files **
	 git diff --staged