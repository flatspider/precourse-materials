- What is git? Why do we need it?

Git is a version control software that allows you to explicitly manage changes to code files. Programmers need it to allow themselves clear control over code changes, feature updates, collaboration, and for history and review processes. Without git, a codebase can change without keeping track of what changed or who changed it. This makes resolving bugs and "rolling back" production breaking errors much more difficult.

- What are the top 10 commands? What do they do?
  <!-- prettier-ignore -->
  The top ten commands for git are:

  1. To pull down a code repository to your local computer, use 'git clone [url]' to copy the code.
  2. To create a new branch, use 'git branch [branchname]'
  3. To switch to an already existing branch, use 'git checkout [branchname]'
  4. To learn about the current state of your code and files, use 'git status' to be informed about which files have been modified and if there is anything to commit, push, or pull.
  5. Once you have established a git repo, use 'git add -A' to add all files in the codebase to the git tracking system.
  6. Once a file has been modified, you can have git keep track of the change by using 'git commit -m "This is what changed"'
  7. Once there are commits, you can use 'git push [remote] [branchname]' to store those changes in the remote location (generally GitHub).
  8. Use 'git pull' to fetch code updates that may have been made by coworkers.
  9. A committed code change can be undone by using the 'git revert [commit hash]' command. This creates a new commit reversing the code changes done in the specified commit.
  10. Once all code is committed and pushed to your feature branch, switch to your main development branch. Then run 'git merge [branchname]' to pull all of the code into the main development branch. This is where you will address any merge conflicts.

- How do you open a PR?

  A pull request (PR) is used after code has been written, committed, and pushed to a smaller feature branch. Now the code needs to be merged into the actual production codebase. This is done using the pull request. They can be created in your git manager (GitHub or similar) in order to create a clean record and discussion of the code changes being merged into production. Go to GitHub.com and navigate to the repo and then branch that has your code commits. Click "compare and pull request". Ensure you select the base branch that you want to merge INTO, and the compare branch that has the code changes you made. Add a title and description, then click "create pull request".
