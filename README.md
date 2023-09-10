# How to use Git and Github in your day-to-day Tutorial for Beginners.

## Summary

- [Introduction](#introduction)

- [Git](#git)

- [GitHub](#github)

- [Why should I use Git?](#why-should-i-use-git)

- [Why should I use GitHub?](#why-should-i-use-github)

- [Installing Git and create a free GitHub account](#installing-git-and-create-a-free-github-account)

- [Git Interfaces (GUI Clients)](#git-interfaces-gui-clients)

- [Setting your username and email in Git](#setting-your-username-and-email-in-git)

- [Setting your Git username and email for every repository on your computer](#setting-your-git-username-and-email-for-every-repository-on-your-computer)

- [Setting your Git username and email for a single repository](#setting-your-git-username-and-email-for-a-single-repository)

- [Create a local repository and adding a new file, let's do it!](#creating-a-local-repository-and-adding-a-new-file-lets-do-it)

- [Git Basic Commands](#git-basic-commands)

- [Initializing a local git repository and starting using Git.](#initializing-a-local-git-repository-and-starting-using-git)

- [Adding a new file to the staging environment (list)](#adding-a-new-file-to-the-staging-environment-list)

- [Create a commit](#create-a-commit)

- [Create a new repository on GitHub](#create-a-new-repository-on-github)

- [Create a new branch](#create-a-new-branch)

- [Push a branch to GitHub Repository](#push-a-branch-to-github-repository)

- [Merge a new branch to a main branch](#merge-a-new-branch-to-a-main-branch)

- [Cloning a entire repository (Clone)](#cloning-a-entire-repository-clone)

- [Forking a entire repository (Fork)](#forking-a-entire-repository-fork)

- [Create a Pull Request (PR)](#create-a-pull-request-pr)

- [Merge a Pull Request (PR)](#merge-a-pull-request-pr)

- [Get changes on GitHub back to your computer (Pull request)](#get-changes-on-github-back-to-your-computer-pull-request)

- [Conclusion](#conclusion)

## Introduction

Hi there, my name is Henrique! 👋

This tutorial teaches you how you can use the **Git** and **GitHub** in your day-to-day.

So, if you're here, I guess that you know what Git and GitHub are, but if you don't know, I will leave below a short resume regarding them.

⬇️

## Git

Git is a distributed, open-source version control system. It enables developers and data scientists to track code, merge changes and revert to older versions. It allows you to sync changes with a remote server as well.

## GitHub

GitHub is a cloud development platform. It is commonly used for saving files, tracking changes and collaborating on development projects. GitHub has become the most popular social platform for software development communities. Individuals can contribute to open-source projects and bug reports, discuss new projects and discover new tools.

## Why should I use Git?

When you use a centralized version control system and decide to use Git, it will change the way that your development team works. Basically, unlike centralized version control systems, Git works like "feature branch workflow", so you can make many Git branches for your future features and it's easy to merge in your main branch as well.

## Why should I use GitHub?

You can use GitHub as a portfolio to show if you are working or studying at the moment. For students, the platform has become a great opportunity to gain work experience and eventually, why not a job opportunity? Below is an example of what the GitHub profile looks like.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364239/Tutorial%20-%20How%20To%20Use%20Git/01-henriqpohl-profile_klkudk.jpg">

# Getting started 🚀

## Installing Git and create a free GitHub account

To get started, the first step to do is, **install git** and **create a free GitHub account**.

<u>**Installing Git:**</u> The latest version of Git is available for **macOS**, **Windows** and **Linux**, to download it, you can use the link below: ⬇️

- [Git Downloads](https://git-scm.com/downloads)

If you want to install by terminal:

<u>**for macOS:**</u>

- **Homebrew**: Install homebrew if you don't already have it, then:

```console
$ brew install git
```

- **MacPorts**:
  Install MacPorts if you don't already have it, then:

```console
$ sudo port install git
```

<u>**for Windows:**</u><br>
You can find the latest version of Git for Windows [here](https://git-scm.com/download/win).

<u>**for Linux:**</u>

**Debian/Ubuntu**
<br>For the latest stable version for your release of Debian/Ubuntu

```console
# apt-get install git
```

For Ubuntu, this PPA provides the latest stable upstream Git version

```console
# add-apt-repository ppa:git-core/ppa
# apt update; apt install git
```

For other Linux distributions you can follow [here](https://git-scm.com/download/linux).

<u>**GitHub account:**</u> After the Git installed, you can create a GitHub account [here](https://github.com/signup).

## Git Interfaces (GUI Clients)

If you've decided not to use GitHub you also can use some Git interfaces, which makes your life easier when you need to see how your repository (project) looks, what was changed in each commit, when it was done, by who and etc.

You can check some Git GUI [here](https://git-scm.com/downloads/guis).

They are available for **Mac**, **Windows**, **Linux**, **iOS** and **Android**.

## Setting your username and email in Git

I strongly recommend that if you've never used Git before, try it. Moreover, it will make your commit list appear with your GitHub username (profile) in your repository, for example, if you don't do this when you make a new commit and send to GitHub repository it will appear like this:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364233/Tutorial%20-%20How%20To%20Use%20Git/02-henriqpohl-git-without-config_w90w6i.jpg">

And after, you can see like this:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364233/Tutorial%20-%20How%20To%20Use%20Git/03-henriqpohl-git-with-config_ovxrxs.jpg">

### Setting your Git username and email for every repository on your computer

Open the Terminal and run the following command: `git config --global user.name` and `git config --global user.name`.
<br>

ℹ️ If you've decided to use GitHub, in this part, you should use the same username and email from your GitHub profile.

- **Setting a Git username:**

```console
$ git config --global user.name "<your-username>"
```

- **Setting a Git email:**

```console
$ git config --global user.email "<your-email>"
```

To confirm that you have set the Git username correctly run the command `$ git config --global user.name` and `$ git config --global user.name`.

```console
$ git config --global user.name
> <your-username>
```

```console
$ git config --global user.email
> <your-email>
```

### Setting your Git username and email for a single repository

Open the Terminal and run the following command `git config user.name` and `git config user.name`.
<br>

- **Setting a Git username:**

```console
$ git config user.name "<your-username>"
```

- **Setting a Git email:**

```console
$ git config user.email "<your-email>"
```

To confirm that you have set the Git username correctly run the command `$ git config user.name` and `$ git config user.name`.

```console
$ git config user.name
> <your-username>
```

```console
$ git config user.email
> <your-email>
```

## Creating a local repository and adding a new file, let's do it!

Open the `Git Bash` already installed in your computer together with Git or you can use `your default Terminal` or `VSCode Terminal`.

```console
cd ~/Desktop
mkdir Tutorial-HowToUseGit
cd Tutorial-HowToUseGit/

~/Tutorial-HowToUseGit %
```

**Adding a new file:** You can use any text editor that you prefer, in this example, to create a new file we will use the `touch <filename>` command:

```console
~/Tutorial-HowToUseGit % touch README.md
~/Tutorial-HowToUseGit % ls
README.md
```

Now, we have the project folder with file (README.MD) inside, ready to go ahead.

💡 TIP: If you are using macOS, I strongly recommend the `Warp Terminal` + `Fish` + `Starship`. You can download it below:

- [Warp](https://www.warp.dev/)
- [Starship](https://starship.rs/)
- [Fish](https://fishshell.com/)

Warp + Fish + Starship are amazing combinations pretty much friendly, take a look in the screenshot below:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364233/Tutorial%20-%20How%20To%20Use%20Git/04-henriqpohl-warp-fish-starship_rhxv8b.jpg">

## Git Basic Commands

- `git init`: create a Git repository in a local directory.
- `git clone <remote-repo-address>`: copy the entire repository from a remote server to remote directory. You can also use it to copy local repositories.
- `git add <file.txt>`: add a single file or multiple files and folders to the staging area.
- `git commit –m "Message"`: create a snapshot of changes and save it in the repository.
- `git config`: used to set user-specific configurations like email, username, and file format.
- `git status`: shows the list of changed files or files that have yet to be staged and committed.
- `git push <remote-name> <branch-name>`: send local commits to remote branch of repository.
- `git checkout -b <branch-name>`: creates a new branch and switches to a new branch.
- `git remote –v`: view all remote repositories.
- `git remote add <remote-name> <host-or-remoteURL>`: add remote server to local repository.
- `git branch –d <branch-name>`: delete the branch.
- `git pull`: fetch commits from a remote repository to a local repository and update it to match that content.
- `git merge <branch-name>`: after resolving merge conflicts the command blends selected branches into the current branch.
- `git log`: show a detailed list of commits for the current branch.

No worries about that for now, we will use all this command together ahead. 😁

## Initializing a local git repository and starting using Git.

**To initialize a git repository:** In the root of the folder, run `git init` command:

As mentioned before, you can use `Git bash`, `your default Terminal` or `VSCode Terminal`.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364233/Tutorial%20-%20How%20To%20Use%20Git/05-henriqpohl-git-init_vzdwnt.jpg">

Git was initialized in your project folder. 🥳

ℹ️ A hidden folder `.git`, was created in your root folder **☠️ never delete it ☠️**, there is where all the Git magic happens.

After initializing the Git repository, you can run `git status` command to see which files git knows exist.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364234/Tutorial%20-%20How%20To%20Use%20Git/06-henriqpohl-git-status_ofkb7b.jpg">

As you can see, Git returned basically "Oh, we have a new file called README.md that you created, but it hasn't been untracked yet."

## Adding a new file to the staging environment (list)

To add a new file to the staging list you can use: `git add <filename>`.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364234/Tutorial%20-%20How%20To%20Use%20Git/07-henriqpohl-git-add_wcliij.jpg">

Now, you can use `git status` to check again.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364236/Tutorial%20-%20How%20To%20Use%20Git/08-henriqpohl-git-add-status_a9ge21.jpg">

You can see now the notice: **"Changes to be committed"** and that Git flagged your file to a **"New file"**, which means that your file is in the staging environment waiting to be committed.

To be easier, look at the image below, you will be able to see how the previous steps works. ⬇️
<br>

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364237/Tutorial%20-%20How%20To%20Use%20Git/09-henriqpohl-how-git-works_scfdl2.jpg">

<br>

## Create a commit

Finally it's time to create your first commit! 😂

Run the following command: `git commit -m "Your message about the commit"`.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364237/Tutorial%20-%20How%20To%20Use%20Git/10-henriqpohl-git-commit_mlxm0w.jpg">

Now, you can see, your **Commit** is done ✅ and your **Branch Master** is available, but we need to do one more thing: We need to rename **Branch Master** to **Branch Main** (that is the currently recommended best practice).

To do that, we will use `git branch` to check what is the current branch name and after `git branch -M "main"` to rename it, take a look in the screenshot below:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364238/Tutorial%20-%20How%20To%20Use%20Git/11-henriqpohl-git-branch_qgkf7v.jpg">

## Create a new repository on GitHub

Now, we will push the local repository to GitHub. You don't need to follow it
if you just want to track your code locally. If you work on a team or want to use your code to collaboratively modify it, you shouldn't skip it.

To create a new repository on GitHub, log in and go to GitHub home page. You should find the “New repository” option under the “+” sign next to your profile picture, on the top right corner of the navbar:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364239/Tutorial%20-%20How%20To%20Use%20Git/12-henriqpohl-button-new-repository_or87dw.jpg">

<br>

If you have already logged in, you can click [here](https://github.com/new).
Both ways will redirect you to the page like below and this is very important because it's where you are going to set your repository name and a short description about it:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364244/Tutorial%20-%20How%20To%20Use%20Git/13-henriqpohl-new-repository_sgd1fh.jpg">

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364245/Tutorial%20-%20How%20To%20Use%20Git/14-henriqpohl-new-repository-created_qcqewl.jpg">

<br>
In this section they show possibilities to start creating a new repository or only make a remote link to an existing Git repository and this is what we will do now.

<br>

To do so, we are going to use the `git remote add origin` and `git push -u origin main`

<br>

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364241/Tutorial%20-%20How%20To%20Use%20Git/15-henriqpohl-git-add-origin-git-push_np4zeo.jpg">

<br>
Now, you can go back to your GitHub repository page to check your push request.

<br>

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364242/Tutorial%20-%20How%20To%20Use%20Git/16-henriqpohl-new-repository-after-push_rewxbb.jpg">

## Create a new branch

When you have a project and you need to make a new feature, but you don't want to make this in the main project while you are developing the feature, for that you can use a branch concept.

Branches allow you to switch between the **"states"** of a project. For example, if you want to add a new page to your website you can **create a new branch** just for that page without affecting the main part of the project. Once you have done it, **you can merge your changes from your branch into the primary branch**. When you create a new branch, Git keeps tracking of which commit your branch **"branched"** off of, so it knows the history behind all the files.

To create a new branch you can run: `git checkout -b <my branch name>`.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364242/Tutorial%20-%20How%20To%20Use%20Git/17-henriqpohl-git-new-branch_vojgxz.jpg">

After creating the new branch, you can use the `git branch` command to confirm that your branch was created.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364242/Tutorial%20-%20How%20To%20Use%20Git/18-henriqpohl-git-branch_k8wyj0.jpg">

## Push a branch to GitHub Repository

After you develop some feature and make a **commit** we'll push the **commit** in your branch with "a new feature" to your GitHub repository, after approved by the repository's owner, the changes can then be **merged** into the **primary branch**, to do so you can use the `git push origin <new-branch-name>` command, GitHub will automatically create the branch for you on the remote repository:

For example take a look in the screenshot below, before, I put some text in my blank README.md file, just to simulate some changes... then:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364237/Tutorial%20-%20How%20To%20Use%20Git/19-henriqpohl-git-push-branch-with-commit_xispcv.jpg">

You might be wondering what the word **"origin"** means in the command above. What happens is that when you clone a remote repository to your local machine, git creates an alias for you. In nearly all cases this **alias** is called **"origin."** It's essentially shorthand for the remote repository's URL. So, to push your changes to the remote repository, you could've used either the command:

```console
git push git@github.com:git/git.git your-branch-name
```

or

```console
git push origin your-branch-name
```

ℹ️ If this is your first time using GitHub locally, it might prompt you to log in with your GitHub username and password.

If you go back in your GitHub repository page, click in **branches**:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364237/Tutorial%20-%20How%20To%20Use%20Git/20-henriqpohl-git-branches-check_k67fuw.jpg">

Now, you'll see your **branch list** with you **last branch** listed there.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364234/Tutorial%20-%20How%20To%20Use%20Git/21-henriqpohl-git-branches-list_vbkbfg.jpg">

## Merge a new branch to a main branch

After you develop the new feature in your new branch, we need to merge to a main branch, to do that, you need to go back to our main branch, then run `git checkout <main branch-name>` and after to merge we need to use `git merge <my-new-branch-name>`

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364234/Tutorial%20-%20How%20To%20Use%20Git/22-henriqpohl-git-checkout-merge-branch_ide8qi.jpg">

After merge, if you refresh the GitHub page, you'll see basically a note saying **"a new branch has just been pushed into the repository"**. You can also click the **"branches"** link to see your branch listed there.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364247/Tutorial%20-%20How%20To%20Use%20Git/23-henriqpohl-new-branch-push_epgro2.jpg">

Now click the green button **"Compare & pull request"** and you're going to make a pull request.

## Create a Pull Request (PR)

A pull request works as an **alert**, after you make a PR, the repository owners will know that you want to make some changes in their project. The owners will make a review in your PR and they will make sure if it looks great before approving your changes on the primary branch.

For example after your `push a new branch` in your own code or `make a new branch in a forked repository` with a collaborator position the owners must see like the screenshot below:

<br>

The PR page shows up before you've submitted it, so you need to send some details to make it easier for the owners to make a review.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364246/Tutorial%20-%20How%20To%20Use%20Git/24-henriqpohl-open-a-pull-request_f08sp9.jpg">

<br>

And this is how it looks like once you've submitted the PR request:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364248/Tutorial%20-%20How%20To%20Use%20Git/25-henriqpohl-review-pull-request_fsteth.jpg">

Now, you can see a big green button that says **"Merge pull request"**. Basically click on it and then click **"Confirm merge"** it means that you've merged and confirmed your changes into the primary branch.

Sometimes you'll be a co-owner or the sole owner of a repository, and in that case you don't need to create a PR to merge your changes. However, it is still a good idea to make one so you can keep a more complete history of your updates. Furthermore, make sure you always create a new branch when making changes because if you have any problem it will be easier to analyze like a "debug".

## Merge a Pull Request (PR)

After clicking the green **"Merge pull request"** button, all your changes in your branch will be merged in the primary branch.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364248/Tutorial%20-%20How%20To%20Use%20Git/26-henriqpohl-git-branch-merged_z9qwgn.jpg">

Once you finish to **merge** the pull request, which means merge some **new branch** to the **main branch**, you no longer need the older version of the branch, so you can delete it. Having many branches can become a big mess, so click in **"Delete branch"** to do it.

Now you can check your commits were merged by clicking on the **"Commits"** in you main page of your repository and you can see the screenshot below:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364243/Tutorial%20-%20How%20To%20Use%20Git/27-henriqpohl-commits-list-after-merged_wbwrms.jpg">

You can also see the hash code of the commit on the right side. A hash code is a unique identifier for each specific commit. It's useful for referring to specific commits and then undoing changes.

To revert you can use: `git revert <hash code number>` command.

## Cloning a entire repository (Clone)

When we need to copy any GitHub repository, we can use `git clone`, but how can we do that? Let's check it below.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364240/Tutorial%20-%20How%20To%20Use%20Git/28-henriqpohl-git-clone_hxguhc.jpg">

After you click on in the green button called **"Code"** you will be able to see and copy the link to clone this repository.

And after in your project folder that you want to clone you can run the command:

```console
git clone https://github.com/henriqpohl/Tutorial-HowToUseGit.git
```

After that, you already have a copy from the desired repository in your computer.

## Forking a entire repository (Fork)

Forking in GitHub is the process of creating a copy of a repository to the user's GitHub Account from another account. It is usually done for community contribution or teamwork.

To make a **Fork** is very easy, go to the repository page that you want to make a **Fork** and click in the **"Fork"** button and after click in **"Create a new fork"** like the screenshot below:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364239/Tutorial%20-%20How%20To%20Use%20Git/29-henriqpohl-create-a-new-fork_nuegfr.jpg">

Once clicked, you will be able to see the **Create a new fork page** like the screenshot below:

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364244/Tutorial%20-%20How%20To%20Use%20Git/30-henriqpohl-create-a-new-fork-form_srgair.jpg">

After that, just click on the green **"Create fork"** button and it will appear in your repositories list.

## Get changes on GitHub back to your computer (Pull request)

This part is very important, now you will get all the changes from your GitHub repository and put it back in your computer because your local code is different from your GitHub repository.

So, you can use: `git pull origin main` or only `git pull`.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364245/Tutorial%20-%20How%20To%20Use%20Git/31-henriqpohl-git-pull_puwg9j.jpg">

The `git pull` command shows you all the files that have changed.

If you want to see all changes you can use the `git log` command to see all new commits.

In this stage you may need to switch branches back to the primary branch. You can do that using the `git checkout main` command.

<img src="https://res.cloudinary.com/dvgb6dadg/image/upload/v1694364246/Tutorial%20-%20How%20To%20Use%20Git/32-henriqpohl-git-log_lumeg3.jpg">

Congratulations! 🥳 <br>
You've successfully made a PR and merged your code to the primary branch.

## Conclusion

https://training.github.com/ <br>
Github’s official git cheat sheets! Handy for remembering the everyday commands you’ll use.

https://git-school.github.io/visualizing-git <br>
Another tool for exploring git visually. This one is more of an open-ended sandbox than learngitbranching.js.org

## Thanks so much!

I hope you learned a lot after reading this, if you have any question you can reach me using my GitHub profile [here](https://github.com/henriqpohl) or in my website [here](https://henriqpohl.com). 😎

Or, if there's something you want me to improve here, why not make a PR? 😜

❤️