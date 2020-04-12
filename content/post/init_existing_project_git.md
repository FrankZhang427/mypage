---
title: "Initialize Git with an existing project"
date: 2020-04-08
tags: ["git"]
draft: false
---

## Initialize Git with an existing project

Here are some steps to initialze an existing project on Github ([Source](https://www.softwarelab.it/2018/10/12/adding-an-existing-project-to-github-using-the-command-line/)):

1. Create a new repository on GitHub. You can also add a gitignore file, a readme and a licence if you want
2. Open Git Bash
3. Change the current working directory to your local project.
4. Initialize the local directory as a Git repository.
    ```
    git init
    ```
5. Add the files in your new local repository. This stages them for the first commit.
    ```
    git add .
    ```
6. Commit the files that you’ve staged in your local repository.
    ```
    git commit -m "initial commit"
    ```

7. Copy the https url of your newly created repo
8. In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
    ```
    git remote add origin remote repository URL
    git remote -v
    ```
9. Push the changes in your local repository to GitHub.
    ```
    git push -f origin master
    ```


This is mainly for easing my own headaches, but I would like to share to anyone who needs it as well.