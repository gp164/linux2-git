# Lab - Git

## Description

This is an individual lab in a group. You do the labs on your local machine and help each other.

## Prerequisites

Account in Github

## Objectives

- Make a pull request on a repository in Github

## Software

git

## TODO

### Using git in a team

#### Create a github account

https://www.wikihow.com/Create-an-Account-on-GitHub

#### Fork this repository `https://github.com/maiyuki/linux2-git`

- Find the fork button in the upper right corner. it will be added to your repository
![](../assets/fork.png)

#### Create new branch and add a file in directory `ADD-YOUR-FILE-HERE/`

- Clone the repository from your repo `<your-github-account>/linux2-git`

- Create a new branch

- create a new file in `ADD-YOUR-FILE-HERE/`

- Make a commit and push

#### Make a pull request to `maiyuki/linux2-git` repository

- Merge your branch to master in the repository in your account (not Mai's)

- Make a pull request to `maiyuki/linux2-git` repository



### Basic git commands (hints)

```bash
git init
git status
git commit
git checkout
git add
git diff
git branch
git merge
git help
```
---

### Answers

#### Create an empty repository and make an initial commit

- Create an empty repository

```bash
git init
```

- Check status

```bash
git status
```

- Create a new file and save

```bash
touch file-1.txt
```

- Check status

```bash
git status
```

- Add file to the index

```bash
git add file-1.txt
```

- Check status

```bash
git status
```

- Make an initial commit

```bash
git commit -m "Init"
```

#### Checkout to a new branch, make changes and merge it back to master

- Checkout a new branch and with a name of choice

```bash
git checkout -b my-new-branch
```

- Create two new files, both with content and save

```bash
echo "My content" > "file-2.txt"
echo "My content again" > "file-3.txt"
```

- Check status

```bash
git status
```

- Add file to the index

```bash
git add .
```

- Check status

```bash
git status
```

- Make a commit

```bash
git commit -m "Added two files"
```

- Make a change in the content of both of the file and save

```bash
echo "More of my content" > "file-2.txt"
echo "More of my content again" > "file-3.txt"
```

- Show changes between commits

```bash
git status
```

- Add file to the index

```bash
git add .
```

- Check status

```bash
git status
```

- Make a commit

```bash
git commit -m "Added changes"
```

#### Merge branch to master

- Check status and verify that there are nothing to be commited

```bash
git status
```

- Check branches merged in master

```bash
git branch --merged master
```

- Checkout to master branch

```bash
git checkout master
```

- Verify that you have master and another branch

```bash
git branch
```

- Verify that you only have the initial file

```bash
ls
```

- Merge branch into master

```bash
git merge my-new-branch
```

- Verify that you have merged

```bash
git branch --merged master
```
