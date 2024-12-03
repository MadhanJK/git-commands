"# git-commands" 

Set global username and email: 

git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"

Set Local Username and Email for a Specific Repository

cd /path/to/your/repo
git config user.name "Your Work Name"
git config user.email "workemail@example.com"

Check Current Git Configuration

git config --list --global  # Shows global config
git config --list           # Shows both global and local config

Repository Setup & Cloning

git init
git clone https://github.com/MadhanJK/git-commands.git

Viewing Repository Status & Logs

git status
git log

Show specific commit details:

git show commitID

Making Changes

git add <filename>       # Add specific file
git add .                # Add all changes in the current directory

Commit changes: 

git commit -m "Commit message describing the changes"

Branching & Merging

git branch <branch-name>

Switch to a different branch:

git checkout <branch-name>

create and switch to a branch in one step:

git checkout -b <branch-name>

List all branches:

git branch

Merge changes from one branch to another: 

git checkout main          # Switch to the target branch
git merge <branch-name>    # Merge changes from the specified branch

Delete a branch: 

git branch -d <branch-name>    # Deletes the local branch

View remote repositories: 

git remote -v

Add a remote repository: 

git remote add origin https://github.com/username/repository.git

Fetch changes from remote repository: Download changes from a remote repository but don’t merge them into your local branch.

git fetch

Pull changes from remote repository: Fetch and merge changes from a remote repository into your current branch.

git pull

Push changes to remote repository: 

git push origin <branch-name>

Push to a remote repository (force push):

git push --force origin <branch-name>

Discard changes in a file:

git checkout -- <filename>

Undo last commit (but keep changes in the working directory):

git reset --soft HEAD~1

Remove untracked files or directories:

git clean -f             # Remove untracked files
git clean -fd            # Remove untracked files and directories

Revert a commit (undo changes from a commit by creating a new commit): 

git revert <commit-hash>

Get help with Git commands: 

git <command> --help
