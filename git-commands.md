             Git Commands Reference

1. Setup & Config -

## git --version
What it does: Shows the installed Git version.
Example: Used to verify git is installed or git version.

## git config
What it does: Sets or updates Git configuration such as username and email.
Example: Used to configure name and email for commits.

## git config --list
what it does: Displays all current Git configuration settings.
Example: used to verify configured name and email.



2. Basic Workflow -
 
## git init
What it does: Initializes a new git repository in the current directory to the staging area.
Example: Used when starting version control for a new project.(jab vcs bnata ha new project k lia)

## git add
What it does: Moves changes to the staging area.
Example: Used to add file to staging area or for changes.

## git commit
What it does: Saves staged changes to the repository history and now changes are tracked.
Example: Used to track files or changes.



3. Viewing Changes - 

## git status
What it does: Shows the current state of files (modified, staged, untracked).  
Example: Used to check what has changed.

## git log
What it does: Displays the commit history.  
Example: Used to review previous commits.

## git log --oneline
What it does: Shows commit history in compact format.  
Example: Used for a quick history overview.

## git diff
What it does:Shows differences between working directory and last commit.  
Example: Used to review changes before staging.

## git diff --staged
What it does: Shows differences between staged changes and last commit.  
Example: Used to review what will be committed.


4. More Commands - 

## git clone <url>: Creates a local copy of a remote repository from a specified URL.

## git push: Uploads committed local changes to the remote repository.

## git pull: Fetches changes from the remote repository and merges them into your current local branch.



@@ Branch Management Commands -

## git branch: Lists all local branches. 

## git branch <branch-name>: Creates a new branch.

## git checkout <branch-name> (or git switch <branch-name>): Switches to a different branch and its also manages files.

## git checkout -b <branch-name>: Creates a new branch and immediately switches to it

## git merge <branch-name>: Integrates changes from the specified branch into the current branch.

## git branch -d <branch-name>: Deletes a local branch (only possible after it has been merged). 

## git switch <branch>: Jump to another branch, use this for switching branches to avoid conflicts.

## git switch -c <branch>: Create a new branch and jump into it.

## git switch -: Go back to the last branch you were using.





