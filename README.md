# How-To-Use-Git
People have been asking me how do I do this in Git?, how do I do that in Git? This will solve those issues.

# Table of Contents

- [Installing Git](#installing-git)
    - [Windows](#windows)
    - [macOS](#macos)
    - [Linux/Unix](#linuxunix)
- [Adding credentials to Git](#adding-credentials-to-git)
    - [Adding username](#adding-username)
    - [Adding password](#adding-password)
    - [Adding email](#adding-email)
    - [Verifying it worked](#verifying-it-worked)
- [Basic CMD/Terminal commands](#basic-cmdterminal-commands)
    - [cd](#cd)
    - [ls](#ls)
    - [touch](#touch)
- [Cloning](#cloning)
- [Initialising Git](#initialising-git)
- [Adding files to be pushed](#adding-files-to-be-pushed)
- [Committing](#committing)
- [Pushing](#pushing)
- [Pulling](#pulling)
- [Author message](#author-message)


## Installing Git
There are many many ways to download Git. 

### Windows
For Windows users, please use [this link](https://git-scm.com/downloads).

### macOS
For macOS, use [Homebrew](https://brew.sh/):
```bash
brew install git
```
or you can use [MacPorts](https://www.macports.org/):
```bash
sudo port install git
```

### Linux/Unix
Using your package manager, install it. Here I will show Debian/Ubuntu as... you'd most likely be on this if you do not know Git.
```bash
sudo apt-get install git -y # -y forces the command to run without you pressing y
# if command failed, run:
sudo apt-get update -y && sudo apt-get upgrade -y
```

## Adding credentials to Git
Adding credentials to Git is as simple as running 3 commands... no, I'm not joking. Make sure you are familiar with your username, email and password for Git.

**Note: These details are for commiting. If you have never ran a Git command, you will be prompted with a very nice GitHub popup!**

### Adding username
```bash
git config --global user.name "The username assigned to you"
```

### Adding password
```bash
git config --global user.name "Your super secret password"
```

### Adding email
```bash
git config --global user.name "hackme@google.com"
```

### Verifying it worked
Just making sure it all worked, enter this command to show that the credentials have been added:
```bash
git config --list
```

## Basic CMD/Terminal commands
To use Git or any CLI program, you *should* have at least a basic understanding of how to move around a command line.

#### cd
To access this repository you have now downloaded, you would have to change into that directory:
```bash
cd not-fake-repo/
# taking the example from above
```

#### ls
"ls" means list. Running this command literally anywhere in your command line will list out all the files and/or folders in your current directory. If there are no files, nothing will be displayed.
There is more of an extended usage of this which would allow you to view hidden files or list a certain directory from it's path:

```bash 
ls # current folder contents

ls ~/Downloads/random_folder # or a specific path

ls -la # or showing hidden files/folders
```

#### touch
No, touch doesn't mean that. It will make a file based on the first parameter you provide. This is handy in a command line interface when you really can't be f\*cked to move to explorer.

```bash 
touch filename.txt # make a file called filename.txt
```

## Cloning
Cloning a Git repository means taking a copy of what is saved online and bringing it to your local drive. 
To clone a *public* repository:
```bash
git clone https://github.com/awesome/not-fake-repo.git
```

To clone a *private* repository:
```bash
git clone https://github.com/awesome/not-fake-repo.git
# you MAY be prompted to enter username and password
# you will not have to if the repo is yours.
```

## Initialising Git
Initialising Git is used when you push files to GitHub. If you have cloned a repository, this will not be needed, but say you accidently delete the `.git/` folder, this will be useful!
```bash
git init
```

## Adding files to be pushed
Adding files is the process of telling Git CLI to add these files when you want to push to a repository.
```bash
git add . # . adds everything in the folder
git add filename.txt # adds certain file and only this
git add folder/ # adds folder+ contents and only this
```

## Committing
When getting ready to push a fix or update to a repository, you've gotta commit to it and mean it! I mean add a message and tell the world, or yourself what you changed.
```bash
git commit -m "your commit message everyone will see :D" # change the message or keep it, your call :D
git commit -am "your commit message everyone will see :D" # -am can also be used to add files.. it's quicker but you do not choose the files
```

## Pushing
It's that time, time for you to push to GitHub and get your project online! This tutorial really hasn't been all that bad right? I hope you've learnt some stuff here and don't ask me in the future.
```bash
git push https://github.com/awesome/not-fake-repo.git # pushing to default branch
git push https://github.com/awesome/not-fake-repo.git master # pushing to master branch
```

## Pulling
Pulling repository files are also needed when you do GitHub stuff. It's really quite useful! It pulls the files from GitHub and appends them to the repository folder on your local device.
```bash
git pull https://github.com/awesome/not-fake-repo.git # and that's all!
```

# Author message
Inf3xt is the author of this repository. Please, if you are wanting to legit copy paste this repository, you credit me. There is a licence for a reason.