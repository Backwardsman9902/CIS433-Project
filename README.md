# CIS433-Project
Collaborative efforts in CIS-433 Project for Group 4

Information about git:

	Process for pushing changes to a branch:
		Run the command 'git add .' from the root of the project to add all folders (you can also add specific folders if you want)
		Run the command 'git commit -m 'Your commit message here'' this will create change locally. Make sure to provide an informative commit message.
		Now choose the correct remote branch name that you want to push to. Make sure to push to your own personal branch. This change will be merged with the master branch later on.
		Run the command 'git push origin <your-branch-name-here>'

	Comparing two branches (usually compare your branch with the master branch)
		From the current branch run 'git diff <branch-to-compare-to>'
		This will show removed data in red and added in green.

	Merging a branch with another branch:
		From <branch1> the branch that you want to change, run the command 'git merge <branch2>' the branch that commits will be pulled from.
		A merge conflict will occur if branch2 is missing commits that branch1 has (branch1 made a change and branch2 does not have that change)
		When a merge conflict occurs you must choose which file to use (from branch1 or branch2) run the command 'git checkout branch-name file-name'
		You must then push the changes after you choose the file on your current branch 'git push origin HEAD'
		If no merge conflict occurs, all you have to do after the merge command is a git push.

	Resetting a Branch to a previous commit:
		Acquire the previous commit id using 'git log'
		Run the command 'git reset --hard <previous-commit-id>
		Run the command 'git push origin HEAD --force' to force overwrite of the current commit with the past commit


