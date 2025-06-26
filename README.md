# Version control

Version control is a system that records changes to files or sets of files over time so that you can recall specific versions later. There are many version control systems, but the most popular one is Git. Git is a **decentralized version control system** that allows multiple developers to work on a project simultaneously without overwriting each other's changes. There are also **centralized version control systems**, but they are less common in modern software development.

## Git and GitHub

Git is a distributed version control system that allows multiple people to work on the same project simultaneously without overwriting each other's changes. It tracks changes in files and coordinates work among multiple people.

GitHub is a web-based platform that uses Git for version control and provides a collaborative environment for developers to share and manage their code.

## Git Installation & Configuration

Download git: [Download](https://git-scm.com/downloads)

```cmd
git config --global user.name "your_username"
git config --global user.email "your_email"
```

## Git Introduction

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

### Branching and Merging

Branching allows you to create a separate line of development in your project. You can create a new branch, switch between branches, and merge changes from one branch to another.

```cmd
git branch <branch_name>  # Create a new branch
git checkout <branch_name> # Switch to a branch
git checkout -b <branch_name> # Create and switch to a new branch
git merge <branch_name>    # Merge changes from a branch
git branch -d <branch_name> # Delete a branch
```

### Undoing Changes

If you make a mistake or want to undo changes, Git provides several commands to help you revert to previous states:

```cmd
git reset <file>          # Unstage a file
git reset --hard HEAD     # Reset the repository to the last commit (discard all changes)
git checkout -- <file>    # Discard changes in a file
git revert <commit>       # Create a new commit that undoes changes from a specific commit
```

### Remote Repositories

Git allows you to work with remote repositories, which are hosted on platforms like GitHub, GitLab, or Bitbucket. This enables collaboration with other developers and teams.
At first you need an  account on one of these platforms.

After that, you can create a new repository and clone it to your local machine. You can also create a new repository on your local machine and push it to a remote platform. Here are some commands to manage remote repositories:

```cmd
git remote add <name> <url>       # Add a remote repository
git remote --set-url <name> <url> # Change the URL of a remote repository
git remote -v                     # List remote repositories
git push <remote> <branch>        # Push changes to a remote repository
git pull <remote> <branch>        # Fetch and merge changes from a remote repository
git fetch <remote>                # Fetch changes from a remote repository
git remote remove <name>          # Remove a remote repository
```

## Git Collaboration

### Cloning a Repository

Cloning a repository allows you to create a local copy of a remote repository. This is useful for contributing to existing projects or starting new projects based on existing code.

To clone a repository, you can use the following command:

```cmd
git clone <repository_url>
```

This command will create a local copy of the repository in a directory with the same name as the repository.

### Forking a Repository

Forking a repository allows you to create your own copy of someone else's project. This is useful for contributing to open-source projects or working on a project without affecting the original codebase.

To fork a repository, you can use the following steps on platforms like GitHub:

1. Go to the repository you want to fork.
2. Click on the "Fork" button in the top right corner.
3. Select your account or organization where you want to fork the repository.

### Create a Pull Request

To propose changes to a project, you can create a pull request. This is typically done on platforms like GitHub, GitLab, or Bitbucket. Here’s how to do it on GitHub:

1. Fork the repository you want to contribute to.
2. Clone your forked repository to your local machine.
3. Create a new branch for your changes.
4. Make your changes and commit them.
5. Push your changes to your forked repository.
6. Go to the original repository on GitHub and click on the "Pull Requests" tab.
7. Click on the "New Pull Request" button.
8. Select your branch and the branch you want to merge into.
9. Add a title and description for your pull request.
10. Click on the "Create Pull Request" button.
11. Wait for the repository maintainers to review your changes.
