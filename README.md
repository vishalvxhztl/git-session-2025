## Understanding origin and Pushing Changes After a Local Commit

### step 1 :

- origin is the default alias for the remote repository from which you cloned or to which you are pushing changes.

- You can check the remote URLs with:
```sh
    git remote -v
```

- if you don't have any origin added

```sh
    git remote add origin <repository-url>

    # to Update remote origin
    git remote set-url origin <new-repository-url>
    # to Remove remote origin
    git remote remove origin
```

### step 2: Steps to Push Changes After a Local Commit

- check your changes are commited

```sh
    git log --oneline --graph --decorate --all
```

or

```sh
    git status
```

- to check current branch name

```sh
    git branch
```

- If the branch already exists remotely:

```sh
    git push origin feature-xyz
```

- If the branch does not exist remotely (first time push):

```sh
    git push -u origin feature-xyz
```
