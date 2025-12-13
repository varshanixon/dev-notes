# GIT
Most widely used Version Control System to maintain working of projects

## BENEFITS OF GIT:
- Simultaneous Development
- Faster Releases
- Built-in Integration
- Strong Community Support
- Pull Requests : A proposal to merge a set of changes from one branch to another

## COMMIT
Every time work is saved, Git creates a commit. A commit is  a snapshot of all files at a point of time.

## BRANCHES
- Each developer saves changes in their own local repository. As a result there can be many different changes based off the same commit. 
- Git provides tools for isolating changes and later merging them back together. Branches manages this separation.
- The git branch command is used to create new branch.
- To toggle between branches we use git switch command, and to merge branch we use git merge.

## WORKING DIRECTORY
- The actual directory where project files are located.
- Modifications made to files in here are 'untracked'.

## STAGING AREA
- also called Index
- Intermediary step between working directory and the Local Repository

## LOCAL REPOSITORY 
- also called .git directory
- It serves as core container for Git's Version Control System
- It stores committed snapshots, manages the project's history and facilitates various Git operations.

## REMOTE REPOSITORY
- Serves as a centralized hubs where team members can push and pull changes, ensuring synchrnized and collaborative development process.

## FILES & COMMITS
- Files in Git are in one of three states: modified, staged or committed.
- When a file is first modified, the changes exist only in the working directory.
- The staging area contains all changes to include in the next commit.The developer stage the changed files to be included in the next commit by git add command.
- Once developer is happy with all the staged files, the files are packaged as a commit with a message describing the change from the staging area to local repository. This commit becomes part of the development history.

## PUSHING
- Developers use git push to transfer commits from local repositories up to centrally hosted remote repositories like GitHub or GitLab.

## PULLING
- git pull fetches the latest changes from the remote repo to the local repo so developers stay up to date.

## INITIALIZING
- The git init command creates a new git repo(local repo)
- It can be used to convert an existing, unversioned project to a Git repo or initialize a new empty repo.
- It creates a .git subdirectory in the current working directory.

