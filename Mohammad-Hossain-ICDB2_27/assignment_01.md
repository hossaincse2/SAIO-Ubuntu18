# Git Commands Scribe Sheet

This scribe sheet includes all the essential Git commands covered in the course and more. Use this as a reference for your version control needs.

## Getting Started with Git

### Configuration
- `git config --global user.name "Your Name"`  
  Sets the name that will be attached to your commits.

- `git config --global user.email "you@example.com"`  
  Sets the email that will be attached to your commits.

- `git config --list`  
  Lists all the Git configurations.

### Initializing a Repository
- `git init`  
  Initializes a new Git repository.

### Cloning a Repository
- `git clone <repository-url>`  
  Clones an existing repository.

## Basic Snapshotting

### Staging and Committing
- `git status`  
  Shows the status of changes as untracked, modified, or staged.

- `git add <file>`  
  Stages a specific file.

- `git add .`  
  Stages all changes in the directory.

- `git commit -m "Commit message"`  
  Commits staged changes with a message.

- `git commit -a -m "Commit message"`  
  Commits all tracked files with a message.

### Viewing History
- `git log`  
  Shows the commit history.

- `git log --oneline`  
  Shows the commit history in a compact format.

- `git log --graph --decorate --oneline`  
  Shows the commit history with a graph of branches.

## Branching and Merging

### Branching
- `git branch`  
  Lists all local branches.

- `git branch <branch-name>`  
  Creates a new branch.

- `git checkout <branch-name>`  
  Switches to the specified branch.

- `git checkout -b <branch-name>`  
  Creates and switches to a new branch.

### Merging
- `git merge <branch-name>`  
  Merges the specified branch into the current branch.

- `git branch -d <branch-name>`  
  Deletes the specified branch.

### Resolving Conflicts
- `git status`  
  Shows files with merge conflicts.

- Edit the conflicted files to resolve the conflicts.

- `git add <file>`  
  Adds the resolved files to the staging area.

- `git commit`  
  Commits the resolved changes.

## Remote Repositories

### Working with Remotes
- `git remote -v`  
  Lists all configured remotes.

- `git remote add <name> <url>`  
  Adds a new remote.

### Fetching and Pulling
- `git fetch <remote>`  
  Fetches changes from the remote.

- `git pull <remote> <branch>`  
  Pulls changes from the remote branch and merges them.

### Pushing
- `git push <remote> <branch>`  
  Pushes local changes to the remote branch.

- `git push -u <remote> <branch>`  
  Sets the upstream branch for the current branch and pushes changes.

## Undoing Changes

### Unstaging and Unmodifying
- `git reset HEAD <file>`  
  Unstages a file.

- `git checkout -- <file>`  
  Discards changes in the working directory.

### Reverting Commits
- `git revert <commit>`  
  Creates a new commit that undoes the changes from the specified commit.

### Resetting
- `git reset --soft <commit>`  
  Resets to a commit, keeping changes in the working directory.

- `git reset --hard <commit>`  
  Resets to a commit, discarding all changes.

## Advanced Topics

### Stashing
- `git stash`  
  Stashes changes in a dirty working directory.

- `git stash list`  
  Lists all stashes.

- `git stash apply`  
  Applies the most recent stash.

- `git stash drop`  
  Deletes the most recent stash.

### Tagging
- `git tag`  
  Lists all tags.

- `git tag -a <tag-name> -m "Message"`  
  Creates an annotated tag.

- `git push <remote> <tag-name>`  
  Pushes a tag to the remote repository.

### Rebasing
- `git rebase <branch>`  
  Reapplies commits on top of another base tip.

### Cleaning
- `git clean -f`  
  Removes untracked files from the working directory.

## Miscellaneous

### Aliases
- `git config --global alias.<alias-name> '<git-command>'`  
  Creates a Git alias for a command.

### Viewing Differences
- `git diff`  
  Shows changes between working directory and staging area.

- `git diff <commit>`  
  Shows changes between working directory and a commit.

## Help
- `git help`  
  Displays help information about Git commands.
 