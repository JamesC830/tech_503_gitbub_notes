# Git and github notes

## Git

### Command flow

Stages:
- Untracked
- Staged
- Commited

```git init```
 
Ititialises the repository (i.e. adds a .git folder)

 ```git add```

Adds files to the staging area

  ```git commit -m "Note```

Commits files to the repository (i.e. saves a snapshot of the current state of the files).
It is good practice to add a note about what you have changed since the last commit.

### Other useful commands

```git status```

Checks the status of files. Will tell what needs to be added to the staging area and wether or not it has been commited

```cd```

Change directorty (use ```cd ..``` to go back one)

``` ls -al```

Tells you what files are in the current directory

### Moving files to Github

You first create a directory in github to be linked to the git directory. From there it will give you the steps you need to follow.

```git remote add origin "link"```

This connects to the github directory. In place of "link", add the link provided by github

```git branch -M main```

Changes the branch name from master to main to ensure continuity between git and github

```git push -u origin main```

Pushes commited files from the main git directory into the gihub directory