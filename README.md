# Create Second Conflict

This is a sample to create a conflict

# Deployment On Github Pages

This Project has been deployed on this link:

https://software-engineering-lab-1402-1403.github.io/Experiment1/

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests] for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

# Developement Details

In the first part we created a new branch to develop the frontend.

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/1.png

Then in the next part we add the new files to git using:
```bash
git add -i
```

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/2.png
https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/3.png

Then we pushed it to the new branch.

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/4.png

Now we Set the project to require pull request before merge like this.

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/6.png

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/7.png

After that we started to create first pull request.

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/5.png

When someone review our pull request we will see something like this:

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/8.png

Then we create .gitignore file and push it like this.

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/9.png

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/10.png

## First Conflict

After we add a fake line in README.md file to make a conflict, we solve it like this:

https://github.com/Software-Engineering-Lab-1402-1403/Experiment1/blob/main/screenshots/13.png

# Questions

## .git Directory

The `.git` folder is a directory in your project that Git uses to store all the metadata and object database for your repository. This includes things like commits, branches, tags, and other information that Git uses to track the history of your project. The `.git` directory is created when you initialize a new Git repository with the command:

```bash
git init
```

## Atomicity in Commits and Pull Requests

Atomicity in the context of atomic commits and pull requests means that each commit or pull request is self-contained and represents a single, complete change. An atomic commit contains a change that is complete in itself and does not leave the codebase in a broken state. Similarly, an atomic pull request consists of one or more commits that together represent a single, coherent change or feature addition to the project.

## Git Commands: Fetch, Pull, Merge, Rebase, and Cherry-pick

- **fetch:** Downloads commits, files, and refs from a remote repository into your local repo. Fetching does not integrate any of these new data into your working files.
- **pull:** Fetches data from a remote repository and then immediately tries to merge it into the current branch. `pull` is essentially a `fetch` followed by a `merge`.
- **merge:** Combines multiple sequences of commits into one unified history. In the simplest cases, it will create a new "merge commit" that combines the histories of the merged branches.
- **rebase:** Reapplies commits on top of another base. It's a way to integrate changes from one branch into another, but unlike merge, it rewrites the commit history to produce a straight, linear succession of commits.
- **cherry-pick:** Allows you to pick a single commit from one branch and apply it onto another. This is useful for applying changes without integrating a whole branch's history.

## Git Commands: Reset, Revert, Restore, Switch, and Checkout

- **reset:** Moves the current branch backward (or forward) to the specified commit, optionally modifying the index (stage) or working directory to match.
- **revert:** Creates a new commit that undoes the changes made in a specified commit, without altering the project history.
- **restore:** Used to restore working tree files. It can undo changes to the contents of the staging area and optionally bring the specified paths back to the version at a given commit.
- **switch:** A relatively new command that switches branches by updating the working directory, and optionally updates some paths in the working directory.
- **checkout:** Used for switching between branches or restoring working directory files. It has been partially superseded by `switch` and `restore` commands in more recent versions of Git.

## Stage (Index)

The stage or index in Git is a staging area where Git stores changes that are about to be committed. Changes added to the index are the ones that will be included in the next commit. This allows developers to choose selectively which changes to commit.

**Stash** is a command that temporarily shelves (or stashes) changes so you can work on a different task. Use:

```bash
git stash
```

to stash your changes, and:

```bash
git stash pop
```

to apply stashed changes back to your working directory.

## Snapshot Concept

In Git, a snapshot refers to the state of a set of files at a particular point in time. When you make a commit, Git essentially takes a snapshot of your files at that moment, and stores a reference to that snapshot. If files have not changed, Git doesn’t store the file again, just a link to the previous identical file it has already stored. Commits in Git are considered snapshots rather than differences or deltas.

## Local vs Remote Repositories

- **Local Repository:** Is a version-controlled project directory on your local machine, managed by Git. It contains all the history, commits, branches, and tags necessary for version control.
- **Remote Repository:** Is hosted on the internet or network for team collaboration. It allows multiple developers to push to and pull from the central repository, enabling collaborative development. GitHub, GitLab, and Bitbucket are examples of services hosting remote repositories.

# Snapshots
