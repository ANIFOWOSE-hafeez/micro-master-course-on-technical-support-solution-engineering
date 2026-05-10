# Git and GitHub

> Learn Git and GitHub as real engineering tools used every day in startups to track changes, collaborate, review work, and ship projects safely.

Git and GitHub are not just “developer tools.”

They are part of how modern startup teams work.

A Technical Support Engineer or Solution Engineer uses Git and GitHub to:
- store project files
- track changes safely
- collaborate with teams
- document solutions
- version scripts and automations
- manage portfolio projects
- show real proof of work

This lesson explains Git and GitHub in a simple, practical way.

---

# Learning Goals

By the end of this lesson, learners should understand:

- what Git is
- what GitHub is
- why version control matters
- how repositories work
- how commits work
- how branches work
- how pull requests work
- how to clone, add, commit, and push
- how to write good commit messages
- how startups use GitHub in practice
- how GitHub helps build a technical portfolio

---

# What Is Git?

Git is a version control system.

It tracks changes in files over time.

Git helps you:
- save progress
- go back to earlier versions
- compare changes
- collaborate with others
- avoid losing work

---

# What Is GitHub?

GitHub is a platform for storing Git repositories online.

It lets you:
- host your code
- share your projects
- collaborate with others
- open issues
- review changes
- use pull requests
- build a public portfolio

---

# Simple Analogy

Think of Git like:
> the system that tracks every draft of your work

Think of GitHub like:
> the online place where that work is stored and shared

---

# Why Git Matters in Startup Work

Startup teams move fast.

People constantly:
- update scripts
- fix bugs
- add features
- edit documentation
- review each other’s work

Git helps teams do this without chaos.

---

# Real Startup Example

A support automation script is helping route tickets.

One engineer updates the script to support a new ticket category.

Another engineer improves the error handling.

A third person updates the documentation.

Git tracks all of these changes cleanly.

Without Git, teams would struggle to know:
- what changed
- who changed it
- when it changed
- whether it works
- how to roll back if needed

---

# Key Git Concepts

---

# Repository

A repository is a project folder tracked by Git.

It usually contains:
- code
- documentation
- config files
- README files
- tests
- assets

Example:
```bash
ai-ticket-router/
```

---

# Working Directory

This is the folder where you edit files on your computer.

You make changes here before saving them to Git.

---

# Staging Area

The staging area is where you prepare changes before committing them.

It acts like a review buffer.

---

# Commit

A commit is a saved snapshot of your project.

It records:
- what changed
- when it changed
- why it changed

---

# Branch

A branch is a separate line of work.

Branches let you build features without breaking the main project.

---

# Main Branch

Usually called:
- `main`
- or sometimes `master`

This branch contains the stable version of the project.

---

# Pull Request

A pull request is a request to merge changes from one branch into another.

It is used for:
- review
- feedback
- collaboration
- quality control

---

# Clone

Cloning copies a repository from GitHub to your computer.

---

# Fork

A fork is a personal copy of someone else’s repository on GitHub.

---

# Add

`git add` tells Git which changes should go into the next commit.

---

# Push

`git push` sends your committed changes from your computer to GitHub.

---

# Pull

`git pull` brings the latest changes from GitHub to your computer.

---

# Why Version Control Is Important

Version control protects you from:
- accidental deletion
- broken updates
- confusion about file versions
- team conflict
- lost progress

This is extremely important in startup environments where systems change constantly.

---

# Installing Git

Check if Git is installed:

```bash
git --version
```

If installed, you will see something like:
```bash
git version 2.x.x
```

---

# First-Time Git Setup

Set your name:
```bash
git config --global user.name "Your Name"
```

Set your email:
```bash
git config --global user.email "your@email.com"
```

Check configuration:
```bash
git config --list
```

---

# Creating a Repository

Go into a project folder and initialize Git:

```bash
git init
```

This creates a hidden `.git` folder that starts version tracking.

---

# Real Startup Example

You may create a repository for:
- a ticket router
- a support dashboard
- a documentation system
- a Python automation script
- a case study portfolio

Git tracks all changes in each project.

---

# Checking Repository Status

```bash
git status
```

This tells you:
- which files were modified
- which files are staged
- which files are untracked

---

# Example Workflow

A normal Git workflow looks like this:

1. edit file
2. check status
3. stage changes
4. commit changes
5. push changes

---

# Creating a File

Example:
```bash
touch README.md
```

Then check status:
```bash
git status
```

Git will show the file as untracked.

---

# Staging Files

```bash
git add README.md
```

To stage everything:
```bash
git add .
```

---

# Committing Changes

```bash
git commit -m "Add project README"
```

Good commits explain what changed.

---

# Good Commit Messages

Good examples:
```bash
git commit -m "Add ticket routing logic"
git commit -m "Fix login validation bug"
git commit -m "Update README with setup instructions"
```

Bad examples:
```bash
git commit -m "update"
git commit -m "stuff"
git commit -m "fix"
```

---

# Why Good Commit Messages Matter

In startup teams, good commit messages help people understand:
- what was done
- why it was done
- how the project evolved

They also help during debugging and code review.

---

# Viewing Commit History

```bash
git log
```

This shows past commits.

For a shorter view:
```bash
git log --oneline
```

---

# Branching

Branches let you work safely.

Example:
```bash
git branch feature/login-fix
```

Switch to the branch:
```bash
git checkout feature/login-fix
```

Or modern version:
```bash
git switch feature/login-fix
```

---

# Why Branching Matters in Startups

If one engineer is changing support automation logic and another is changing the README, branches keep work separate and safe.

This prevents:
- broken production code
- accidental overwrites
- merge confusion

---

# Merging Branches

Once a feature is ready, merge it back into main.

Example:
```bash
git checkout main
git merge feature/login-fix
```

---

# Real Startup Workflow

Typical team flow:
- create branch
- build feature
- test feature
- open pull request
- request review
- merge into main

---

# GitHub Collaboration Features

GitHub adds collaboration tools on top of Git.

Important GitHub features include:
- repositories
- pull requests
- issues
- project boards
- code review
- discussions
- actions
- releases

---

# Pull Requests

Pull requests are one of the most important team workflows.

They help teams:
- review code
- discuss changes
- catch mistakes
- approve updates
- keep main branch clean

---

# Real Startup Example

A solution engineer builds a support dashboard.

They open a pull request so:
- another engineer can review
- product can check the workflow
- support can confirm the logic
- documentation can be updated

---

# Issues

GitHub issues are used to track:
- bugs
- tasks
- improvements
- feature requests
- documentation updates

Example issue:
> Add support for high-priority ticket alerts

---

# README Files

README files explain your project.

They usually contain:
- overview
- setup
- usage
- features
- tech stack
- screenshots
- impact
- future improvements

This is very important for portfolios.

---

# Why GitHub Matters for Your Career

GitHub is more than a code hosting platform.

It is also:
- a portfolio
- a collaboration proof
- a documentation hub
- a hiring signal
- a project history

Recruiters and startup founders can inspect your GitHub to see:
- how you think
- how you document
- how you structure work
- how you solve problems

---

# GitHub for Technical Support and Solution Engineering

You can use GitHub to show projects like:
- AI ticket router
- endpoint health monitor
- onboarding automation
- cloud backup monitor
- internal support knowledge base
- security compliance tracker

Each project should look polished and professional.

---

# Important Files in a GitHub Project

| File | Purpose |
|---|---|
| `README.md` | project explanation |
| `.gitignore` | files Git should ignore |
| `requirements.txt` | Python dependencies |
| `Dockerfile` | container setup |
| `.env.example` | sample environment variables |
| `LICENSE` | usage rights |

---

# `.gitignore`

This file prevents sensitive or unnecessary files from being tracked.

Examples to ignore:
- `.env`
- virtual environments
- caches
- logs
- temporary files

---

# Real Security Rule

Never commit:
- API keys
- passwords
- tokens
- credentials
- private config files

Use:
- `.gitignore`
- environment variables
- `.env.example`

---

# GitHub Profile Importance

Your GitHub profile can become part of your professional brand.

A strong GitHub profile shows:
- clean project structure
- clear documentation
- active repositories
- consistent work
- useful technical projects

---

# Practical Git Workflow for Beginners

---

# Step 1 — Create a folder

```bash
mkdir my-project
cd my-project
```

---

# Step 2 — Initialize Git

```bash
git init
```

---

# Step 3 — Create files

```bash
touch README.md
```

---

# Step 4 — Check status

```bash
git status
```

---

# Step 5 — Stage changes

```bash
git add README.md
```

---

# Step 6 — Commit changes

```bash
git commit -m "Add README file"
```

---

# Step 7 — Connect GitHub remote

```bash
git remote add origin https://github.com/username/repo.git
```

---

# Step 8 — Push changes

```bash
git push -u origin main
```

---

# Common Git Commands

| Command | Purpose |
|---|---|
| `git init` | start Git tracking |
| `git status` | check file status |
| `git add` | stage files |
| `git commit` | save snapshot |
| `git push` | upload to GitHub |
| `git pull` | download latest changes |
| `git branch` | manage branches |
| `git merge` | combine branches |

---

# Git Mistakes Beginners Make

| Mistake | Better Approach |
|---|---|
| Skipping commits | Commit regularly |
| Bad commit messages | Write clear messages |
| Pushing secrets | Use `.gitignore` |
| Working on main only | Use branches |
| Ignoring status | Check `git status` often |
| No README | Document your work |

---

# Real Startup Story Example

A support automation script works locally, but a teammate breaks it with a rushed change.

Because the code is in Git:
- the team can inspect what changed
- compare branches
- revert the issue if needed
- recover quickly

That is why Git matters in production environments.

---

# GitHub and Career Growth

If used properly, GitHub can help you show:
- technical discipline
- teamwork readiness
- documentation habits
- project ownership
- startup thinking

---

# Beginner Exercise

## Task 1
Initialize a repository.

## Task 2
Create a `README.md`.

## Task 3
Add and commit the file.

## Task 4
Make a second change.

## Task 5
Commit again with a better message.

---

# Beginner Project Idea

## GitHub Profile Setup Project

Build a professional GitHub profile with:
- profile README
- pinned projects
- consistent commit history
- clean repository organization
- strong README documentation

---

# Real Skills Built Here

This lesson develops:
- collaboration habits
- version control discipline
- documentation quality
- project organization
- professional workflow understanding

These are critical for:
- support engineering
- solution engineering
- automation
- startup team collaboration
- technical portfolio growth

---

# Key Takeaways

- Git tracks changes over time
- GitHub stores and shares Git repositories online
- Branches protect work
- Pull requests support collaboration
- Good commit messages matter
- GitHub is also part of your portfolio
- Every technical professional should use Git well

---

# Next Lesson

Continue to:

```bash
markdown.md
```

The next lesson explains:
- Markdown formatting
- headings
- lists
- links
- code blocks
- tables
- why Markdown is essential for GitHub documentation
