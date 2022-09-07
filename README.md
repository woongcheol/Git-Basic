`latest update : '22. 9. 7.`

![image](https://user-images.githubusercontent.com/86638578/184536737-4fd185c4-09f9-4228-9ddd-ad6f6ec05c6c.png)
</br>

## 개요
#### ✔ Learn how to manage source code for collaboration.
#### ✔ To do this, learn about GitHub's commands and how to deal with certain situations.
</br>

## Contents
### Branch
#### 1. Create
#### 2. Delete
#### 3. Rename
#### 4. List
#### 5. Merged
</br>

### Repository
#### 1. Connect local repository with remote repository
#### 2. Connect local branch with remote branch
</br>

### Reset
#### 1. Undo git add before a commit
#### 2. Undo git push
</br>

## Branch
#### Create
  ```
  git branch <branch name>
  ```
#### Delete
  ```
  git branch -d <branch name>
  ```
#### Rename
  ```
  git branch -m <current branch name> <new branch name>
  ```
- use the -M option, overwritten an existing branch with same name
#### List
  ```
  git branch
  ```
- add the -v option, check local branch and last commit
- add the -r option, check remote branch
- add the -a option, check local / remote branch
#### Merged
  ```
  git branch (-merged | -no-merged)
  ```
## Reset
#### To undo git add before a commit
  ```
  git reset HEAD <file>
  ```
- don't add the file name, all the files you add will be undo
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
#### Create local branch associated with remote branch
  ```
  git checkout --track <remote branch>
  ```
#### Delete remote branch
  ```
  git push origin --delete utility
  ```