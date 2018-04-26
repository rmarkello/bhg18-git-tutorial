# BHG18 Montreal Collaborative git/GitHub Tutorial

## Terminology
* **FORK**: Make a personal, editable copy of a public GitHub repository. Refers to both the act of making and the copy itself.
* **CLONE**: Download the contents of an online git repository onto your local computer.
* **BRANCH**: Create a parallel copy/trajectory of a git repository. Refers to both the act of creating and the copy itself.
* **CHECKOUT**: Switch to a different *branch* of your git repository.
* **STAGE**: Prepare new/deleted/modified files to be *committed* to git history.
* **COMMIT**: Store all *staged* changes in git history. Refers to both the act of storing and the changes themselves.
* **COMMIT MESSAGE**: Information about the changes being stored in git history with a *commit*. Generally, this should start with a short summary of the changes made, followed by a blank line, and then a more in-depth description of the changes.
* **REMOTE**: An online version of your local git repository.
* **PUSH**: Send changes of a local git repository back to the *remote* copy of the repository (e.g., the copy on GitHub that was *cloned*).
* **PULL**: Copy down changes from a *remote* a git repository to your local version.
* **PULL REQUEST (PR)**: Request a different *fork* or *branch* integrate the changes you've made in your git repository. Refers to both the act of requesting and the request itself.
* **MERGE**: Join two branches of a git repository together.

## GitHub collaborative workflow
1. First, `fork` the project you want to work on so you can have your own copy of the original repository. Do this by going to the repository on GitHub and clicking `fork` in the top-right corner.

2. Copy the `fork` to your computer by opening a terminal and typing: `git clone https://github.com/yourusername/reponame`. A new directory will be created titled `yourreponame` with the contents of the repository.

3. Open [Atom](https://atom.io/), click *File --> Add a project folder*, and select the folder `yourreponame`. A directory tree should show up on the lefthand side of the window with the contents of the repository.

4. Create a new `branch` by clicking the tab in the lower, lefthand corner that reads 'Master'. Click 'New Branch', type the name of your new `branch` (something descriptive of the changes you intend to make, like "new-feature-X"), and press 'Enter' on your keyboard.

5. Make some changes to the code or files in the repository!

6. Type 'ctrl + shift + 9', which will open up the Git tab on the righthand side of the window (or click *Packages --> GitHub --> Toggle Git Tab*). This tab is what you'll use to `stage` and `commit` your changes to git history.

7. Right click on the files in the "Unstaged changes" window that you've added/deleted/modified and click "`Stage`". They should move down to the "Staged changes" window, below.

8. Type a `commit message` that describes the changes you made! It should ideally started with a short, one-line summary (about 60 characters) of the change you made, followed by a blank line, and then a more in-depth description of those changes.

9. Click '`Commit` to XXX', where XXX is the name of the branch you created, to `commit` the changes to history.

10. Next, we need to `push` the changes we made back to the GitHub copy of the repository. Click the tab with a down and up arrow in the lower, lefthand corner of the Atom window. You may see a warning that says 'Note: No remote detected for branch XXX. Pushing will set up a remote tracking branch on remote repo "origin".' When we created a branch in step 4, that branch was only made in the local (`cloned`) copy of our repository; the GitHub copy of the repository (our `remote` copy) was not automically updated to reflect this new branch. Click "`Push`" to copy both the new branch and your changes up to your `remote` repository.

11. Using a web browser, navigate to `https://github.com/yourusername/reponame`, the URL used in step 2. 

12. If you are logged in to your GitHub account, you should see a status update with a yellow background noting that changes were recently pushed to a new `branch`! Click "Compare and `pull request`" on the righthand side of that yellow status update.

13. Select the `fork` / `branch` that you want to make a `pull request` onto. The fork could be the original repository that you `forked` in step 1, or your copy of it. Generally, if you are contributing to someone else's project, you will want this to be the original repository. The branch should usually be `master`, but if you are contributing to someone else's project ask them what they would like!

14. Click 'Create `pull request`', enter some information about the `pull request` (describing what changes you made), and then click 'Create `pull request`', again. If you are contributing to someone else's project, they would generally either provide feedback on your changes and request edits or `merge` them!
