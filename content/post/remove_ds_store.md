---
title: "Remove .DS_Store files from Git"
date: 2020-04-04
tags: ["git", "macOS"]
draft: false
---

## Remove .DS_Store files from Git

It gets annoying when you see a ```.DS_Store``` file in every single directory after you push to a git repository. Luckily, we can use ```.gitignore``` to ignore them when you commit your changes. I found a pretty good solution on [Stack Overflow](https://stackoverflow.com/questions/107701/how-can-i-remove-ds-store-files-from-a-git-repository):

Remove existing files from the repository:

```bash
find . -name .DS_Store -print0 | xargs -0 git rm -f --ignore-unmatch
```

Add the line

```bash
.DS_Store
```

to the file ```.gitignore```, which can be found at the top level of your repository (or created if it isn't there already). You can do this easily with this command in the top directory

```bash
echo .DS_Store >> .gitignore
```

Then

```bash
git add .gitignore
git commit -m '.DS_Store banished!'
```

This is mainly for easing my own headaches, but I would like to share to anyone who needs it as well.

