# Github-Guide
Github Pushing  guide

1.	Create a new repository on GitHub. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub. 

2.	Open Git Bash.

3.	Change the current working directory to your local project.

4.	Initialize the local directory as a Git repository.
$ git init -b main

5.	Add the files in your new local repository. This stages them for the first commit.
6.	$ git add .
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.

7.	Commit the files that you've staged in your local repository.

8.	$ git commit -m "First commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.

9.	At the top of your GitHub repository's Quick Setup page, click  to copy the remote repository URL. 

10.	In the Command prompt, add the URL for the remote repository where your local repository will be pushed.

11.	$ git remote add origin  <REMOTE_URL> 

12.	# Sets the new remote

13.	$ git remote -v
# Verifies the new remote URL

14.	Push the changes in your local repository to GitHub.

15.	$ git push origin main
--------------------------------
# for merging and fetching the github 

git fetch origin main
git merge origin master

# 
After to wrote this code I received other error: (non-fast-forward)

I write this code:

git fetch origin main:tmp
git rebase tmp
git push origin HEAD:main
git branch -D tmp

## forcely pushing 

git push --force origin main

