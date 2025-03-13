# Workflow and branching using Git
Github works in strict collaboration with the Git VCS, a Distributed Version Control system; this means that each time we want to make a change on a file's project we will be able to download our project's repository, make a mess of it on our remote machine and, in case our changes are helpful, add them on the actual project by merging the file we modified.

We just performed two actions:
- We created a branch on our project, so there are a moment in time where there are two identical projects (one in our machine and one on the server) and the following moment our copy is slightly different from the original one.
- We merged the changes (after confirming that they work, or in slang, to make a commit), modifying the server's repository too.

### Creating branches on Github
Even if Git is a very powerful tool, it's not really necessary to create a new branch or merge an existing one; so, there's a guide on how to do it directly from Github:
- Go to the Code Tab and click on the "Branches" button on the top left of the screen.
- The last option on the drop-down menu shows all branches; click it.
- A new menu is opened, still under the Code Tab. There, we can create a new branch by clicking the "New Branch" button on the top right.
- After naming our new branch, we can select it as our workspace, creating a new repository with the same files of when we branched the main.
- When we are ready, we can go back to the Branch Tab, click on the settings on the right side of our branch and create a pull request.

## Git
Now we can start to work on our project using Git:
1. Create a clone of the repository.
    - On the Code Tab, click the green "Code Button" on the top-right of the screen.
    - Copy the URL in the clipboard.
    - Reach in your computer the folder where you want to copy your repository, right click and open the folder with your terminal.
    - In the terminal, type `git clone <clone-URL>`.
    - The clone is now created correctly.
2. Control the cloned repository status.
    - By using the command `git status` in the terminal it's possible to retrieve some information on our cloned repository, such as the branch we are working on, if this branch is up to date with the main, if there are commits to send and the status of our working tree.
3. Editing a file.
    - We can create a file directly with Git, or add one after creating it.
    - By using the command `git add <namefile>` we add the file on the branch we're actually working on. This file is actually in a particular location called "staging area", where all the changes to every file are stored before we commit them.
    - To commit all our changes we just type the command `git commit -a`, and the modified files will now be in our local repository.
4. Pushing the changes to the remote repository.
    - Once we are **completely** sure our changes are correct, we can use a pull request to push them into the remote repository (in this case on Github); to do so, we'll need the command `git push origin main`.   
