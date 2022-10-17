# How-To-Use-Git
People have been asking me how do I do this in Git?, how do I do that in Git? This will solve those issues.

# Table of Contents

- [Installing Git](#installing-git)
    - [Windows](#windows)
    - [macOS](#macos)
    - [Linux/Unix](#linux/unix)


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

