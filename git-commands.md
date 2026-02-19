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



@@ Remote Synchronization -

## git clone <url>: Creates a local copy of a remote repository from a specified URL.

## git push: Uploads committed local changes to the remote repository.

## git push origin [branch-name]: Uploads your local branch commits to the remote repository.

## git pull: Downloads updates from the remote repository and automatically merges them into your current branch.

## git fetch: Downloads changes from the remote but does not update your local code until you merge them.

## git remote -v: Lists all remote repositories linked to your local project. 



@@ Inspection (Looking at History)

## git log: The standard history view. Shows commit hashes, authors, and dates.

## git log --oneline --graph --all: The "Pro View." Shows a compact, visual map of all branches and how they connect.

## git show <commit-hash>: Deep dive into one specific commit to see exactly which lines changed.

## git diff: Shows the difference between your current files and the last saved state.

## git diff --staged: Shows what you’ve added to the "waiting room" but haven't committed yet.

## git blame <file>: Shows who changed every single line of a file and when (great for debugging "who broke this?").



@@ Undoing Changes (The Fixers)

## git restore <file>: The "Delete My Mess" command. It wipes away unsaved changes in a file and reverts it to the last committed version.

## git restore --staged <file>: Keeps your code changes but takes the file out of the "ready to commit" area.

## git commit --amend -m "new message": Fixed a typo in your last commit message? This overwrites it so no one ever knows.
## git revert <commit-hash>: The Safe Undo. It creates a new commit that does the exact opposite of a previous commit. Best for shared projects.

## git reset --soft HEAD~1: Undo the last commit, but keep your work in the staging area. Use this if you committed too early.

## git reset --hard HEAD~1: The Nuclear Option. Deletes the last commit and destroys all the code in it. Cannot be easily undone.


@@ The "Save for Later" Undo

## git stash: Not exactly an undo, but it clears your "messy" working directory by hiding changes in a temporary vault.

## git stash pop: Brings those changes back when you're ready.



@@ Advanced Maneuvers (Moving Specific Work)

## git cherry-pick <commit-hash>: Applies the changes from a specific commit onto your current branch.

## git cherry-pick <hash1> <hash2>: Grab multiple specific commits at once.

## git cherry-pick --continue: Use this if you hit a conflict while picking and have finished fixing it.

## git cherry-pick --abort: If the pick is too messy and you want to go back to exactly how things were before you tried. 
