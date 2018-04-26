# BHG18 Montreal Collaborative git/GitHub Tutorial

## Terminology
* **ATOM**: A text editor with git/GitHub integration
* **FORK**: Make a personal, editable copy of a public GitHub repository. Refers to both the act of making and the copy itself.
* **CLONE**: Download the contents of an online git repository onto your local computer.
* **BRANCH**: Create a parallel copy/trajectory of a git repository. Refers to both the act of creating and the copy itself.
* **CHECKOUT**: Switch over to a different *branch* of your git repository.
* **STAGE**: Prepare new/deleted/modified files to be *committed* to git history.
* **COMMIT**: Store all *staged* changes in git history. Refers to both the act of storing and the changes themselves.
* **COMMIT MESSAGE**: A 
* **REMOTE**: An online version of your local git repository.
* **PUSH**: Send changes of a local git repository back to the *remote* copy of the repository (e.g., the copy on GitHub that was *cloned*).
* **PULL**: Copy down changes from a *remote* a git repository to your local version.
* **PULL REQUEST (PR)**: Request a different *fork* or *branch* integrate the changes you've made in your git repository. Refers to both the act of requesting and the request itself.
* **MERGE**: Join two branches of a git repository together.

## GitHub collaborative workflow
1. Always `fork` a project you want to work on, so you can have your own copy of the original repository. Do this by going to the repository on GitHub and clicking `fork` in the top-right corner.
2. Making sure you have git installed on your computer, open a terminal and type: `git clone https://github.com/yourusername/reponame`. A new directory will be created titled `yourreponame`.
3. Open [Atom](https://atom.io/), click **File --> Add a project folder**, and select the folder `yourreponame`.
