Git and GitHub Cheat Sheet
Basic Git Commands
1. Configuration
bash
Copy code
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
Configure Git with your name and email.

2. Initialize a Git Repository
bash
Copy code
git init
Initializes a new local Git repository in the current folder.

3. Clone a Repository
bash
Copy code
git clone <repository-url>
Clones an existing repository from GitHub or another remote location.

4. Check Repository Status
bash
Copy code
git status
Displays the status of changes in your working directory.

5. View Changes
bash
Copy code
git diff
Shows changes in the files that are not staged yet.

6. Add Files to Staging Area
bash
Copy code
git add <file-name>   # Add a specific file
git add .             # Add all changed files
Adds files to the staging area (preparing for a commit).

7. Commit Changes
bash
Copy code
git commit -m "Commit message here"
Records changes from the staging area into the local repository.

8. View Commit History
bash
Copy code
git log
Shows the commit history for the current branch.

9. Branching and Merging
Create a New Branch

bash
Copy code
git branch <branch-name>
Switch to a Branch

bash
Copy code
git checkout <branch-name>
Create and Switch to a Branch

bash
Copy code
git checkout -b <branch-name>
Merge a Branch into Current Branch

bash
Copy code
git merge <branch-name>
10. Deleting a Branch
bash
Copy code
git branch -d <branch-name>
Deletes a local branch.

GitHub Commands
11. Push Changes to Remote Repository
bash
Copy code
git push origin <branch-name>
Pushes committed changes to GitHub on a specific branch.

12. Pull Latest Changes from Remote
bash
Copy code
git pull origin <branch-name>
Fetches and integrates changes from the remote repository to your local repository.

13. Fork a Repository on GitHub
Go to the repository on GitHub and click the "Fork" button.
14. Submit a Pull Request
On GitHub, after pushing changes, go to the repository and click on "Compare & pull request."
Undoing Changes
15. Unstage a File
bash
Copy code
git reset <file-name>
Removes a file from the staging area without deleting the changes.

16. Undo Last Commit (Keep Changes)
bash
Copy code
git reset --soft HEAD~1
Moves the last commit back to the staging area but keeps the changes.

17. Discard Changes in Working Directory
bash
Copy code
git checkout -- <file-name>
Reverts changes in a file back to the last commit (local).

Remote Repositories
18. Add Remote Repository
bash
Copy code
git remote add origin <remote-repo-url>
Adds a new remote repository (e.g., GitHub) for pushing/pulling changes.

19. View Remote Repository
bash
Copy code
git remote -v
Lists the remote repositories associated with the local repository.

20. Remove Remote
bash
Copy code
git remote remove <remote-name>
Removes a remote repository.

Stashing and Reverting
21. Stash Changes
bash
Copy code
git stash
Temporarily save changes that are not yet ready to be committed.

22. Apply Stashed Changes
bash
Copy code
git stash apply
Restores the most recent stashed changes.

23. Revert a Commit
bash
Copy code
git revert <commit-id>
Creates a new commit that undoes the changes from a previous commit.

Tagging
24. Create a Tag
bash
Copy code
git tag -a v1.0 -m "Version 1.0"
Creates an annotated tag (useful for versioning releases).

25. Push Tags to Remote
bash
Copy code
git push origin --tags
Pushes all local tags to the remote repository.

Collaboration Workflow
26. Collaborating with Others
Fork the repository (on GitHub).
Clone your fork.
Create a Branch for your feature or bugfix.
Commit your changes.
Push your branch to GitHub.
Submit a Pull Request.
Resolving Merge Conflicts
27. Resolve Merge Conflicts
Open the conflicted files.
Look for conflict markers like:
plaintext
Copy code
<<<<<<< HEAD
// Your changes
=======
// Changes from the other branch
>>>>>>> branch-name
Edit the file to resolve the conflicts, then:
bash
Copy code
git add <file-name>
git commit
Quick Summary of Commands
Command	Description
git init	Initialize a local Git repository
git clone <url>	Clone a repository
git add <file>	Stage changes
git commit -m "message"	Commit changes
git push origin <branch>	Push changes to GitHub
git pull origin <branch>	Pull changes from GitHub
git branch <name>	Create a new branch
git checkout <name>	Switch to a branch
git merge <branch>	Merge a branch
git log	View commit history
git stash	Temporarily save changes
git revert <commit>	Revert to a specific commit
git reset --soft HEAD~1	Undo last commit but keep changes staged
git remote add <name> <url>	Add a new remote repository
This cheat sheet covers the essentials of working with Git and GitHub. You can use it as a quick reference for everyday Git tasks!
