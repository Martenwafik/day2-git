# Git & GitHub - Lab 2 Documentation

## 📌 Project Overview
This repository contains the practical implementation of Lab 2. The project demonstrates practical knowledge of Git workflows, including branching, merging, remote repository management, and tagging.

---

## 🌿 Part 1: Branching, Merging, and Collaboration

### 1. Project Setup & Initial Push
Created the local repository, added the initial files, and pushed to the remote repository:
```
git init
touch README.md
git add README.md
git commit -m "Initial commit"
git remote add origin <remote-repository-url>
git push -u origin main
```
## 2. Creating Branches (dev & test)
Created two branches, added a unique file to each, and pushed them to the remote repository:


### Setting up 'dev' branch
```
git checkout -b dev
touch dev-file.txt
git add dev-file.txt
git commit -m "Add dev file"
git push -u origin dev
```
### Setting up 'test' branch
```
git checkout main
git checkout -b test
touch test-file.txt
git add test-file.txt
git commit -m "Add test file"
git push -u origin test
```
## 3. Merging Branches into Main
Merged the changes from both dev and test branches into the main branch locally, then pushed the updates:

```
git checkout main
git merge dev
git merge test
git push origin main
```
## 4. Branch Cleanup
Removed the dev and test branches locally and remotely to maintain a clean repository history:

### Delete branches locally
```
git branch -d dev
git branch -d test
```
### Delete branches remotely
```
git push origin --delete dev
git push origin --delete test
```
## 5. Collaboration
Sent a repository invitation to the required email (shimaakhallaf507@gmail.com) via GitHub Settings -> Collaborators.

# 🏷️ Part 2: Version Tagging and Markdown
## 1. Creating and Pushing an Annotated Tag
Created an annotated tag for version 1.7 and pushed it to the remote repository:

```
git tag -a v1.7 -m "Release version 1.7"
git push origin v1.7
```
## 2. Listing and Deleting Tags
Commands to list existing tags and remove them both locally and remotely:


### List all tags
```
git tag
```
### Delete tag locally
```
git tag -d v1.7
```
### Delete tag remotely
```
git push origin --delete v1.7
```
## 3. Markdown Formatting
Added a local image into this README.md file using the following Markdown syntax:

Markdown
![ITI Logo](iti-logo.png)
