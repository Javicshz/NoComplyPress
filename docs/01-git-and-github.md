# Command Terminal & GitHub Basics: A Beginner’s Guide

  

Welcome to the Git & GitHub basics guide! This README is designed to help you get started with Git and GitHub. Follow these steps to understand the fundamentals and learn how to work with a repository.

Read this entire page because it is the first step to collaborating together for the project. You must learn to ***"Clone the repo"*** to your local computer. Once you have cloned the repo you must then:

 1. Learn how to <b>pull</b> updates from the main branch
 2. Create your own <b>branch</b>
 3. <b>Checkout</b> your own branch (switch to your own branch to ensure you do not make any changes to the main branch)
 4. Check that you are on your own branch by using ```git branch```
 5. Add your updates to your own branch using ```git add .```
 6. Commit your changes and write a message using ````git commit -m " "````
 7. <b>push</b> your changes into the main branch after ensuring there is no conflict.
 
The listed steps to learn above are just the basic most useful commands we will be using with github.

  

## 1. What is Git and GitHub?

  

-  **Git** is a version control system that lets you track changes in your code and collaborate with others.

-  **GitHub** is an online platform that hosts Git repositories. It makes it easy to share your code, collaborate, and keep your work backed up online.
- Github is a little hard to understand at first but once you work on it for a while, things become easier to understand. Practice makes perfect!

You can use the [Github Desktop Website](https://desktop.github.com/download/) but I highly suggest using the command terminal which this document is intended to teach.

Windows, Linux and Mac's all have a command terminal. Windows might also have it listed a Powershell. You will want to learn some basic commands to learn to navigate your command terminal. 
# Basic Command Line Navigation and File Commands (Windows / Mac / Linux)

All major operating systems Windows, macOS, and Linux have a command terminal. Windows may show it as **Command Prompt** or **PowerShell**. These basic commands will help you navigate, create, and manage files and folders across different systems.

I would suggest creating a folder in your documents files that you can use to experiment with these commands.

## Navigation Commands

| Action               | Windows Command        | macOS / Linux Command |
|----------------------|-------------------------|------------------------|
| Show current folder  | `cd`                    | `pwd`                  |
| List files/folders   | `dir`                   | `ls`                   |
| Change directory     | `cd foldername`         | `cd foldername`        |
| Go up one directory  | `cd ..`                 | `cd ..`                |

---

## Creating Files and Folders

| Action                   | Windows Command          | macOS / Linux Command |
|--------------------------|---------------------------|------------------------|
| Create folder            | `mkdir foldername`        | `mkdir foldername`     |
| Create empty file        | `type nul > file.txt`     | `touch file.txt`       |

---

## Deleting Files and Folders

| Action                        | Windows Command              | macOS / Linux Command     |
|-------------------------------|-------------------------------|----------------------------|
| Delete file                  | `del file.txt`                | `rm file.txt`              |
| Delete folder (empty)       | `rmdir foldername`            | `rmdir foldername`         |
| Delete folder (with files)  | `rmdir /s foldername`         | `rm -r foldername`         |

---

## Extra Helpful Commands

| Action                          | Windows Command         | macOS / Linux Command     |
|----------------------------------|--------------------------|----------------------------|
| Clear screen                   | `cls`                   | `clear`                    |
| See command help               | `command /?`            | `man command`              |
| Copy file                      | `copy file1.txt file2.txt` | `cp file1.txt file2.txt`   |
| Move or rename file            | `move old.txt new.txt`     | `mv old.txt new.txt`       |
---


This cheat sheet gives you a solid base to work in any terminal environment, whether you're using Git, setting up a project, or exploring the filesystem.

# Basic Git and GitHub Commands

This guide covers the essential Git commands for working with a GitHub repository. It assumes you already have Git installed and that you're working inside a Git-tracked project folder.

---

## Initial Setup

| Action                          | Command                                  |
|----------------------------------|-------------------------------------------|
| Set your name (one-time)        | `git config --global user.name "Your Name"` |
| Set your email (one-time)       | `git config --global user.email "you@example.com"` |
| Check config                    | `git config --list`                        |

---

## Starting a New Project

| Action                          | Command                                  |
|----------------------------------|-------------------------------------------|
| Initialize Git in a folder      | `git init`                                |
| Check Git status                | `git status`                              |
| Add all files to staging        | `git add .`                               |
| Add a specific file             | `git add filename.txt`                    |
| Commit your changes             | `git commit -m "Your commit message"`     |

---

## Working with a GitHub Repository

| Action                             | Command                                                      |
|------------------------------------|---------------------------------------------------------------|
| Clone a remote repo                | `git clone https://github.com/user/repo.git`                 |
| Add a remote origin (after init)  | `git remote add origin https://github.com/user/repo.git`     |
| Push local repo to GitHub         | `git push -u origin main`                                    |
| Pull latest changes               | `git pull origin main`                                       |

---

## Branching (Optional, Advanced Later)

| Action                         | Command                        |
|--------------------------------|--------------------------------|
| Create a new branch            | `git branch feature-branch`    |
| Switch to that branch          | `git checkout feature-branch`  |
| Create and switch at once      | `git checkout -b feature-branch` |
| Merge branch into main         | `git checkout main` → `git merge feature-branch` |

---

## Undo & Fix Mistakes

| Action                          | Command                            |
|----------------------------------|-------------------------------------|
| Unstage a file                  | `git reset filename.txt`            |
| Undo last commit (keep changes) | `git reset --soft HEAD~1`           |
| Discard local changes           | `git checkout -- filename.txt`      |
| See commit history              | `git log`                           |

---

## Tips

- Always pull before you push: `git pull origin main`
- Use meaningful commit messages
- Don't force push unless you know what you're doing

---

# Git/GitHub Terms + Login Setup

This guide explains the common Git terms you'll run into, and how to set up your GitHub login so you don't have to type your username and password every time you push code.

---

## Common Git Terms (In Plain English)

| Term        | What It Means |
|-------------|----------------|
| **Git**     | A tool that tracks your code changes so you can go back in time or collaborate with others. |
| **GitHub**  | A website where your Git-tracked code lives online. You can push to it, pull from it, and share with others. |
| **Repository (repo)** | A folder that Git is tracking. It could be local (on your computer) or remote (on GitHub). |
| **Commit**  | A saved checkpoint of your project. It includes a message describing what you changed. |
| **Staging area** | A place where changes are prepped before committing. Think of it like organizing before saving. |
| **Branch**  | A copy of your code that you can edit without affecting the main version. Used for experimenting or adding features. |
| **Merge**   | When you bring changes from one branch into another. Often used to combine feature branches into `main`. |
| **Push**    | Upload your commits from your computer to GitHub. |
| **Pull**    | Download commits from GitHub to your computer (in case something changed online). |
| **Origin**  | The default name Git gives to the remote repo (usually on GitHub). It's where your code pushes/pulls from. |
| **Main**    | The primary branch of most repos (used to be called `master`). |

---

## How to Log In to GitHub via Terminal (And Avoid Typing Passwords Every Time)

GitHub removed password login via terminal for security reasons. Now we use **Personal Access Tokens (PAT)** instead.

### Step 1: Make Sure Git Is Set Up

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```


## Create a Personal Access Token (PAT) For Github

To avoid logging in every time you push to GitHub, you can generate a **Personal Access Token** and save it to your system.

### Where to Go
- Visit: [GitHub Token Settings](https://github.com/settings/tokens)

### 1. Start the Process
- Choose **"Fine-grained tokens"** or **"Classic tokens"**
- Click **"Generate new token"**

### 2. Fill in Token Info
- **Name:** Something like `NoComplyPress Access`
- **Expiration:** Choose 90 days or "No expiration"

### 3. Select Scopes (Permissions)
- `repo` — full access to repositories
- `workflow` — *(optional)* if you're using GitHub Actions

### 4. Generate and Save
- Click **Generate Token**
- **Copy the token** immediately — you won’t be able to view it again.

> **Tip:** Paste it into your password manager or a secure note for safekeeping.


