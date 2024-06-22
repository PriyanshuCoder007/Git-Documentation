# Learn from this documentation

## Configure tooling

### Configure user information for all local repositories

      $ git config --global user.name "[name]"

      $ git config --global user.email "[email address]"

      $ git config --global color.ui auto

## Branches

### Branches are an important part of working with Git. Any commits you make will be made on the branch you’re currently “checked out” to. Use git status to see which branch that is.

    $ git branch [branch-name]

    $ git switch -c [branch-name]

    $ git merge [branch]

    $ git branch -d [branch-name]

## Create repositories

### A new repository can either be created locally, or an existing repository can be cloned. When a repository was initialized locally, you have to push it to GitHub afterwards.

    $ git init

    $ git remote add origin [url]

    $ git clone [url]

    The .gitignore file

    Sometimes it may be a good idea to exclude files from being tracked with Git. This is typically done in a special file named .gitignore. You can find helpful templates for .gitignore files at github.com/github/gitignore.

## Synchronize changes

### Synchronize your local repository with the remote repository on GitHub.com

    $ git fetch

    $ git merge

    $ git push

    $ git pull

## Make changes

### Browse and inspect the evolution of project files

    $ git log

    $ git log --follow [file]

    $ git diff [first-branch]...[second-branch]

    $ git show [commit]

    $ git add [file]

    $ git commit -m "[descriptive message]"

## Redo commits

### Erase mistakes and craft replacement history

    $ git reset [commit]

    $ git reset --hard [commit]

## Glossary

        git: an open source, distributed version-control system
        GitHub: a platform for hosting and collaborating on Git repositories
        commit: a Git object, a snapshot of your entire repository compressed into a SHA
        branch: a lightweight movable pointer to a commit
        clone: a local version of a repository, including all commits and branches
        remote: a common repository on GitHub that all team members use to exchange their changes
        fork: a copy of a repository on GitHub owned by a different user
        pull request: a place to compare and discuss the differences introduced on a branch with reviews, comments, integrated tests, and more
        HEAD: representing your current working directory, the HEAD pointer can be moved to different branches, tags, or commits when using git switch
