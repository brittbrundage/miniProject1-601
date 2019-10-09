**Git Commands**
<br>

- **Repository:** It is a git/file location where all the files are stored.

	- _Example:_ A repository tracks all changes made to file in the project, building a history over time. Meaning, if you delete .git/ folder, then you delete your projects history.

- **Clone (git clone ):** It is a command line utility that is used to target an existing repository and create a clone or copy of the target repository.

	- _Example:_ Make a clone of a repository in a new directory at another location. The original repository can be located on the local filesystem or on remote machine.

- **Fork:** It is a copy of a repository that allows you to freely experiment with changes without affecting the original project.

	- _Example:_ A developer create a fork copy in their local system.

- **Branch (git branch):** A git branch command lets you create, list, rename and delete branches in the current repository.
	- _Example:_ A branch represents an independent line of development.

- **Commit (git commit):** A git commit command is used to save changes to the local repository.
	- _Example:_ the command git commit -m Êtype your message∆ records or snapshots the file permanently in the version history.

- **Merge (git merge):** Allow to combine multiple sequences of commits into one unified history.
	- _Example:_ the command git merge (branchName) lets you take the independent lines of development created by git branch and integrate them into a single branch.

- **Checkout:**  It is used to switch from one branch to another.
	- _Example:_ the git checkout (branchName) command lets you navigate between the branches created.

- **Push:** It is to push commits made on your local branch to a remote repository.
	- _Examples:_
                - The git push (variable name) master command sends the committed changes of master branch to your remote repository.
                - The git push (variable name) branch command sends the branch commits to your remote repository
                - The git push -all (variable name) command pushes all branches to your remote repository
                - The git push (variable name) : (branchName) command deletes a branch on your remote repository.

- **Pull:** It is used to fetch and download content from a remote repository and immediately update the local repository
to match that content.
	- _Example:_ git  pull command update current local branch and update the remote tracking branches for all othe branches.

