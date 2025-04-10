# Git-Workflow Documentation

This document outlines the git workflow used for this project.
It includes all the the git commands and steps I followed from project setup to completion.

## 1. Initializing the project

I initialized Git in the project folder so that git can start tracking it for me.

```bash
git init
```

## 2. Project Setup

- I staged my files.
- Did my first commit.
- Set "main" as the main upstream branch, instead of "master"s
- And then linked my local repo to the remote repo.

```bash
git add .
git commit -m 'first commit'
git branch -M main
git remote add origin <remote repo link>
```

## 3. Created Feature Branches

Then I went ahead to create feature branches for each particular feature or section I worked on to keep track of my progress categorically...

```bash
git branch <New Feature Branch Name>
```

Afterwards, I made sure to publish the feature branch from the local repo to the remote repo, while setting it as the upstream, so that all the follow-up pushes will go into that feature branch automatically

```bash
git push -u origin <feature Branch Name>
```

Afterwards, I went to github to make a PR for the completed feature branch to be reviewed and merged into the main branch

Afterwards I also made sure to switch back to the local main branch to pull the recent changes, then create next branch off the main branch

```bash
git checkout main
git pull
git checkout -b <new Branch Name>
```

## 4. Occasional Git Commands Used

Below are some of the basic git commands I used throughout the proces...

```bash
git status
git log
git switch
git branch
```
