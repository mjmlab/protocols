# Forking and contributing to a lab Git repo on GitHub: `mjmlab/protocols` as an example

This is a bit meta: a protocol to demonstrate how to contribute to the protocols. It also serves as a model for working with other lab repositories.

- [What is a repository/repo?](#what-is-a-repositoryrepo)
- [Git vs Github](#git-vs-github)
- [Git and GitHub Setup and Basic Commands](#git-and-github-setup-and-basic-commands)
	- [GitHub signup](#github-signup)
	- [Play with GitHub](#play-with-github)
	- [Set Up a Text Editor on your computer](#set-up-a-text-editor-on-your-computer)
	- [Install Git on your computer](#install-git-on-your-computer)
	- [Play with Git](#play-with-git)
	- [Some notes about local Git repos:](#some-notes-about-local-git-repos)
- [Forking and cloning the `protocols` repo](#forking-and-cloning-the-protocols-repo)
	- [Fork the repo to your GitHub account](#fork-the-repo-to-your-github-account)
	- [Upstream vs Remote vs Local versions of the repo](#upstream-vs-remote-vs-local-versions-of-the-repo)
	- [Modify a lab protocol](#modify-a-lab-protocol)
	- [Short commit message](#short-commit-message)
	- [Pull Request: Now suggest this change to the lab](#pull-request-now-suggest-this-change-to-the-lab)
- [Dealing with the situation where your Remote repo (`mandel01/protocols`) is different from the lab Upstream repo (`mjmlab/protocols`)](#dealing-with-the-situation-where-your-remote-repo-mandel01protocols-is-different-from-the-lab-upstream-repo-mjmlabprotocols)

## What is a repository/repo?

A repository (repo) in a directory or folder in which `Git` is tracking changes. It is an effective method for version control and to collaborate on code and documents.

## Git vs Github

Git is the language that facilitates the change tracking and merging. GitHub is a git server and associated website that facilitates collaboration and posting online.

## Git and GitHub Setup and Basic Commands

You can use Git on your own computer without the need for GitHub. However, since GitHub is a pretty and easy-to-use interface we will start there and then move to the command line Git interface on our computer.

### GitHub signup

1. [Sign up](https://github.com/join) for a GitHub account.  
1. [Sign up](https://education.github.com/discount_requests/new) for the GitHub educational discount.  
  - This will allow you to have private repos at no cost.  
1. Email Mark with your GitHub username so you can be invited to the [lab GitHub group](https://github.com/mjmlab).  

### Play with GitHub

See additional resources below to complete the following steps:

1. Look at the [Markdown language](https://daringfireball.net/projects/markdown/syntax), including the syntax particular for GitHub, aptly called [GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/). The syntax is fairly simple, and this is widely used in GitHub documents, including our protocols.
1. Create a repo in your account via the web interface.
1. Make a change to the repo. This is called a "commit".
1. View the commit history of your repo.

### Set Up a Text Editor on your computer

Recommendation is `Atom`

1. [Download `Atom`](https://atom.io).
1. Install Atom (or move to `Applications` folder on Mac).

### Install Git on your computer

1. On Mac, type `git config` on the command line (e.g., `Terminal` app) and if it is not installed you will be prompted to install the `XCode command line tools`, which includes `Git`.
1. [Here is information for other platforms](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and more detailed information for Mac.
1. Set up global Git settings (don't type the dollar signs...):

```
$ git config --global user.name "Your name here"
$ git config --global user.email "your_email@example.com"
```

Configure Atom to be the default text editor for Git:

```
$ git config --global core.editor "atom --wait"
```

### Play with Git

Make a directory to store your repos locally and then move into that directory:

```
$ mkdir ~/code
$ cd ~/code
```

Clone your new GitHub repo to your computer (here I am using a repo called `testrepo`).

```
$ git clone https://github.com/mandel01/testrepo.git
```

Navigate into the repo directory

```
$ cd testrepo
```

Make a change to the repo using the command line.  `git add`, `git commit`, `git status`:

```
$ touch newfile.md
$ git add newfile.md
$ git commit -m 'Add newfile.md'
[master 02501e7] Add newfile.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 newfile.md
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working directory clean
```

Push the change to the origin repo.  `git push`:

```
$ git push origin master
Counting objects: 2, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 328 bytes | 0 bytes/s, done.
Total 2 (delta 0), reused 0 (delta 0)
To https://github.com/mandel01/testrepo.git
   69c9980..02501e7  master -> master
```

The `origin master` part means that the change is being pushed out to the repo's `origin`, on the branch called `master`, which is the default branch. If we are unsure of what origin (Git server or other location) we are using, we can check the origin with `git remote`:

```
$ git remote -v
origin	https://github.com/mandel01/testrepo.git (fetch)
origin	https://github.com/mandel01/testrepo.git (push)
```

Additionally, `git pull` will pull information from that GitHub remote repo to your local repo.


Finally, create a repo on your computer via the command line. Here I'll create a repo in a new directory called `lovinsquid`:

```
$ cd ~/code
$ mkdir lovinsquid
$ cd lovinsquid
$ lovinsquid git init
Initialized empty Git repository in /Users/markmandel/code/lovinsquid/.git/
```

Add some files to the directory and the check the status with `git status`:

```
$ touch file1.md file2.md file3.md
$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	file1.md
	file2.md
	file3.md

nothing added to commit but untracked files present (use "git add" to track)
```

Add these files to the repo and commit them as above. Here we can use the dot `.` to commit all uncommitted files in the current directory:

```
$ git add .
$ git commit -m 'Add important files'
[master (root-commit) 2937708] Add important files
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 file1.md
 create mode 100644 file2.md
 create mode 100644 file3.md
$ git status
On branch master
nothing to commit, working directory clean
```

Now this directory is being tracked by Git on our computer. It can then be pushed to GitHub in the future, or never!

### Some notes about local Git repos:

1. Subdirectories and files within a Git-tracked directory will be analyzed by commands such as `git status` but are not actually in the repo until you `git add` them. Therefore, there is no version tracking until they are added.
1. Use can use a [`.gitignore` file](https://help.github.com/articles/ignoring-files/) to tell Git to ignore certain classes of files/folders. You can then proceed to add all files/folders with `git add .` but Git will know to ignore the items in the `.gitignore`.
1. Keep Git repos separate. It is not good practice to nest a Git repo within another Git repo.
1. A major benefit of Git is branches, but that will be described elsewhere (or use the Google).

Other resources for Git and GitHub:

- http://kbroman.org/github_tutorial/pages/resources.html

Finding the url to clone any GitHub repo:

![](images/github/github-clone-https.png)





## Forking and cloning the `protocols` repo

### Fork the repo to your GitHub account

Go to https://github.com/mjmlab/protocols

Click on "Fork".

![](images/github/fork1.png)

Select your personal account (if relevant).

![](images/github/fork2.png)

The virtual copy machine will appear, and then you will have a forked version.

![](images/github/fork3.png)

Some relevant items to note:

![](images/github/your-fork.png)

```
mandel01/protocols
forked from mjmlab/protocols
```
These are two separate repos now. `mjmlab/protocols` is the lab protocols repo. `mandel01/protocols` is my forked copy of the lab protocols. I can change mine, the lab can change its version, and they can be separate for their whole lives! Of course, that is not the point here. A major advantage of using Git/GitHub is the ability to merge changes that different people make.

You can then ask, is my forked repo different from the lab repo?

```
This branch is even with mjmlab:master.
```

Nope. This line means that they are the same.


### Upstream vs Remote vs Local versions of the repo

In this setup where there is a central lab repo, your forked repo, and (later) a local copy of the repo on your computer, we will refer to:

Name          | What                                | Detail
------------- | ----------------------------------- | ------
 **UPSTREAM** | central repo (GitHub)               | https://github.com/mjmlab/protocols.git
 **REMOTE**   | your fork (Github)                  | https://github.com/mandel01/protocols.git
 **LOCAL**    | local clone of your fork (Computer) | git clone https://github.com/mandel01/protocols.git

(substitute your username for `mandel01`)

Note that in this setup, changes made to your Local or Remote repo can be synchronized to each other using commands on the previous page, `git push` / `git pull`. For more complicated commands


### Modify a lab protocol

We noticed some typos in the "Squid Colonization" protocol. Here we are going to edit the `squid-colonization.md` Markdown file directly in GitHub. We will proceed to "commit" the changes to our repo. We will then proceed to suggest the changes to the lab repo, in a process called a "Pull Request" ("Hey lab, we request that you pull in these changes!").

In our Remote, click on the file to edit.

![](images/github/select-file.png)

Click on the pencil icon to edit the file.

![](images/github/edit-file.png)

Make the desired changes using [GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/).

![](images/github/edit-markdown.png)

For each change, you can use GitHub's built-in preview functionality.

![](images/github/edit-markdown-view.png)

When you have completed the changes, Add a short commit message and (if needed) more detailed information.

![](images/github/commit-message.png)

### Short commit message

**Correct text formatting in squid-colonization.md**
- Maximum 50 characters
- Use the imperative ("Change microliters" not "Changed..." or "I changed"...)
- No period

Commit extended description can be used if needed. [Additional information about commit messages here](http://chris.beams.io/posts/git-commit/) and [here](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).


Your Remote will now be 1 change ahead of the Upstream:

![](images/github/one-ahead.png)

### Pull Request: Now suggest this change to the lab

Note that if you have other protocols to edit, you can do all of them, and then include them all in a Pull Request.

Click on the button labeled "Pull Request" (see above).

You will see the changes suggested, with the new lines in Green and the old lines in Red.

![](images/github/pr1.png)

You can also display the "Rich Diff", which will show the changes in a more granular way.

![](images/github/pr2.png)

Click Create Pull Request, edit/add any information (again use the guidelines above for commit messages).

![](images/github/pr3.png)

![](images/github/pr4.png)

If you permission to merge changes into `mjmlab/protocols` then you will have the option to Merge Pull Request immediately. If not, then an owner on that account will be notified that your Pull Request is waiting.

![](images/github/pr5.png)

Additional discussion can proceed about the Pull Request. You will automatically be notified of any discussion, and if you want to alert someone specifically you can include their GitHub username preceded by an `@`, as in this example. That person can then comment on the proposed changes before they are merged.


## Dealing with the situation where your Remote repo (`mandel01/protocols`) is different from the lab Upstream repo (`mjmlab/protocols`)

In this example there have been some changes made to the Upstream that are not in the Remote repo.

![](images/github/behind1.png)

Note: Be sure that you do not lose anything that you have changed (i.e., if your repo is **ahead** of the lab upstream repo).

We need to update our Remote repo so that it matches the lab repo, before we make any further changes. Surprisingly, this cannot really be done on GitHub and requires the following steps using a Local version of the repo. [Detailed help is here](https://help.github.com/articles/syncing-a-fork/) and the specific steps for this example are listed below:


Clone the Remote repo (if you have already cloned it, then `git pull` your changes locally to pull in any changes on your remote).

```
$ cd ~/code
$ git clone https://github.com/mandel01/protocols.git

```

Move into the repo:

```
$ cd protocols
$ git status
On branch master
Your branch is up-to-date with 'origin/master'.
nothing to commit, working directory clean
```

Note that the Git status is up-to-date because **it is comparing the Local with the Remote**.

Now we need to add the Upstream:

```
$  git remote -v
origin	https://github.com/mandel01/protocols.git (fetch)
origin	https://github.com/mandel01/protocols.git (push)
$ git remote add upstream https://github.com/mjmlab/protocols.git
$ git remote -v
origin	https://github.com/mandel01/protocols.git (fetch)
origin	https://github.com/mandel01/protocols.git (push)
upstream	https://github.com/mjmlab/protocols.git (fetch)
upstream	https://github.com/mjmlab/protocols.git (push)
```

Excellent! Now we can work on merging the Upstream into our Local, and then re-synchronize the Local & Remote.

```
$ git fetch upstream
remote: Counting objects: 3, done.
remote: Compressing objects: 100% (1/1), done.
remote: Total 3 (delta 2), reused 3 (delta 2), pack-reused 0
Unpacking objects: 100% (3/3), done.
From https://github.com/mjmlab/protocols
 * [new branch]      master     -> upstream/master
$ git checkout master
Already on 'master'
Your branch is up-to-date with 'origin/master'.
$ git merge upstream/master
Updating a0b9be1..f11628d
Fast-forward
 gibson-assembly.md | 128 +++++++++++++++++++++++++++++++++++++++++---------------------------------------
 1 file changed, 66 insertions(+), 62 deletions(-)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working directory clean
$ git push origin master
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 917 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To https://github.com/mandel01/protocols.git
   a0b9be1..f11628d  master -> master
```
