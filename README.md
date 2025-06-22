# Introduction to version control

Version control is a system that records changes to files or sets of files over time so that you can recall specific versions later. There are many version control systems, but the most popular one is Git. Git is a **decentralized version control system** that allows multiple developers to work on a project simultaneously without overwriting each other's changes. There are also **centralized version control systems**, but they are less common in modern software development. 

## Introduction to Git and GitHub

Git is a distributed version control system that allows multiple people to work on the same project simultaneously without overwriting each other's changes. It tracks changes in files and coordinates work among multiple people.

GitHub is a web-based platform that uses Git for version control and provides a collaborative environment for developers to share and manage their code.

## Git Installation & Configuration

Download git: https://git-scm.com/downloads

```cmd
git config --global user.name "your_username"
git config --global useremail "your_email"
```

## Git Crash Course

### Basic Commands

Initialize a new Git repository or clone an existing one - use the following commands:

```cmd
git init <directory>    # Initialize a new Git repository
git clone <repository>  # Clone an existing repository
```

After you have a repository, you can start tracking changes to files. Here are some basic commands to get you started:

```cmd
git add <file>          # Stage changes for commit
git commit -m "message" # Commit staged changes with a message
git status              # Check the status of the repository    
git log                 # View commit history
```



