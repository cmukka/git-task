# git-task
To introduce folks to git version control system and github

# Introduction
Go through this to understand more: [Introduction](http://stackoverflow.com/questions/11816424/understanding-the-basics-of-git-and-github).

We'll be uploading with a proper introduction shortly.

# Instructions
These are for folks using Linux, Mac OSX. Windows people have to download git bash separately.

## Basic Procedures
* Make a new repository in your account
  * There will be an option `Initialize with README`. Check that option.


* There are two methods to have a local repository in your machine
  1. First method
    * `git clone <url>` where \<url\> is the url of the repository you initialized. Eg. \<url\> for this repository is `https://github.com/cmukka/git-task`. 
    * With this, a clone of the repo on github will be created 


  2. Second method
    * Create a folder(repository) in your machine: `mkdir <reponame>`
    * Navigate into the directory: `cd <reponame>`
    * Initialize it as a git repository: `git init`
    * Link it with the online repository: `git remote add origin <url>` where \<url\> is the url of the repository you initialized.
    * Add some random files in the repository.
    * Add the files for staging for the next commit: `git add .`.
    * Commit(Save) the files: `git commit -m <message>` where \<message\> is in double quotes and can be anything to describe your commit.
    * Push it to your online repository: `git push origin master`
      * You'll end up with an error message saying that your local repository is not up-to-date with your online(remote) repository. This happens, because you have a README.md in the online repo which is not present in your local repository.`git pull origin master` will pull all the contents from the online(remote) repo to your local repo. Now proceed with: `git push origin master`


## Making Contributions
### Basic
* Make a fork of this repository
* Clone your fork to your device (`git clone <url>` where \<url\> is the url of the forked repository that is in your account and not `https://github.com/cmukka/git-task`)
* Create a new branch named `contrib` (`git checkout -b contrib`)
* Create a new file named `yourname.txt` in intro directory with your name and Birthdate as the content (refer to yash.txt for an example)
* Commit (`git add .` & `git commit -m <message>`) the changes and push it to your fork `git push origin contrib` (read it as push the contrib branch to the remote named origin)
* Browse to your repository on Github and submit a pull request
