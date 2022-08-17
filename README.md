`latest update : '22. 08. 17.`

![image](https://user-images.githubusercontent.com/86638578/184536737-4fd185c4-09f9-4228-9ddd-ad6f6ec05c6c.png)
</br>

## 개요
#### ✔ Learn how to manage source code for collaboration.
#### ✔ To do this, learn about GitHub's commands and how to deal with certain situations.
</br>

## Contents
### Repository
#### 1. Connect local repository with remote repository
#### 1. Connect local branch with remote branch
</br>

### Reset
#### 1. Undo git add before a commit
#### 2. Undo git push
</br>

## Reset
#### To undo git add before a commit
  ```
  git reset HEAD <file>
  ```
- If you don't add the file name, all the files you add will be undo
#### To undo git push
  ```
  git reset <commit id> // or HEAD^
  git commit -m "Write commit messages"
  git push -f
  ```
## Repository
#### Connect local repository with remote repository
  ```
  git remote add origin <git url>
  ```
#### Connect local branch with remote branch
  ```
  git checkout <branch>
  git branch --set-upstream-to <remote branch>
  ```