# Getting started with `git`

> **NOTE**: 
> - Make sure that you have `git` on your machine. You can check it by open cmd and type `git`+`Enter`. If `git` is on your machine you will see all basic information about your current `git` version. If not please install `git` from <https://git-scm.com/download/win>.
> - We recommend to work with GitHub in VS code. You can download VS code (VSC) from https://code.visualstudio.com/ and the extension for GitHub from https://code.visualstudio.com/docs/editor/github (there you will find also some usefull instructions for working with GitHub in VS Code).
> - For more informations about GitHub please visit the official GitHub Documentation (https://docs.github.com/en).


## 1. Fork the repository
A `fork` is basically a *special* clone of the repository: when you create a `fork`, a new repository is created in *your* GitHub account, which is linked to the main one. You have now full control of this repository (your are the admin), but you can still see if changes are made in the main repo and in case sync this changes with your version (see below). Most importantly, you can change the code yourself without interfering with other people work. To fork a repository follow the instruction:
1. Got to the the repository, which you want to `fork` (here: `02_CMM_Usermat` from the `kfmResearch-NumericsTeam`)
2. Click on `Fork` on the top right - and it's done.

## 2. Clone the (forked) repository in VSC
1. Create a folder on your computer where you want to save your cloned respository (e.g. in C:\code).
2. Open the `terminal` in VSC, type `cd C:\code` and press `Enter`.
3. Type `git clone https://github.com/WeberMarius/CMM_Usermat.git` (here we clone the CMM_Usermat repository - You will find the .git link in the (cloned!) repository 
4. Now you can open the Foler in `C:\code` and work on it in VSC.

## 3. Pull requests from VSC 
However, at some point you might want to merge your code into the main or cloned repository. This is done creating a so called `pull request`You can chose between merge only to your cloned repo or to merge it with the main repository. If the latter is used, you are asking the main developer to review your code and merge it into the main repository. 

[<img src="https://github.com/kfmResearch-NumericsTeam/03_Coding_Induction/blob/main/01_Git/00_Figures/Pull%20request%20to%20your%20cloned%20repository.jpg">](https://github.com/kfmResearch-NumericsTeam/03_Coding_Induction/blob/main/01_Git/00_Figures/Pull%20request%20to%20your%20cloned%20repository.jpg)


## 4. Working with commands
All the stuff mention above you can do with the VSC GUI or by using `git` commands 
We collect some important commands, which you will run all the time to keep track of your local repository and sinc it with the remote 

1. `git remote -v` -> List the current configured remote repository for your fork.
2. `git remote add upstream <https://user@github.com/main-repository-address>` -> adds a pointer to the main repository so you can do all the `reading` operations you would normally do with your own repository (fetch and pull).
3. `git fetch upstream` -> Fetch the branches and their respective commits from the upstream repository
4. `git pull upstream <branch>` -> merge the latest changes from the main repo

1. `git fetch` -> get the latest changes without merging
2. `git pull` -> get the latest changes and merge them
3. `git status` -> check if there are changes to the repo
4. `git add .` -> stage all the changes
5. `git commit -am "\<message>"` -> commit all staged changes (save the status of the repo at that time)
6. `git push` -> send the you commits to the origin

## Git tools

Even though learning the basic commands can be extremelly usefull, when things get complicated (merging, resolving conflicts, visualising the log history, etc.) it is a good idea to use external tools designed to work with git.

Here, we suggest two main tools (but many others are available)

### GitKraken

This software is free to use for public repos for everyone. For students and university members the pro version is available for free, which allows to use its functionalities also for private repos.

You can download the software here: <https://www.gitkraken.com/download>

On the website there are plenty of videos that explain the software and git concepts in general, which I strongly reccomend to watch.

[<img src="https://www.gitkraken.com/img/index/gk-product-2.png">](GitKraken)

### vscode

In vscode git is already integrated, but we suggest to enhance the basic functionalities with the `gitgraph` extension <https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph>

[<img src="https://github.com/mhutchie/vscode-git-graph/raw/master/resources/demo.gif">](git_graph)

