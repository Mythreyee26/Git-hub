 Navigate to the **Code** tab of the class repository on GitHub.
1. Click the green **Code** button.
1. Copy the **clone URL** to your clipboard.
1. Open your command-line application.
1. Retrieve a full copy of the repository from GitHub: `git clone <CLONE-URL>`
1. Once the clone is complete, navigate to the new directory created by the clone operation: `cd <REPOSITORY-NAME>`

### Our favorite Git command: `git status`

git branch
git branch --all
git branch -a

git switch <BRANCH-NAME>


1. First, let's check the status of our working tree: `git status`
1. Move the file from the working tree to the staging area: `git add my-file.md`
1. Let's see what happened: `git status`
1. Now let's take our first snapshot: `git commit`
1. Git will open your default text editor to request a commit message. Simply type your message on the top line of the file. Any line without a # will be included in the commit message.
1. Save and close the commit message
1. Let's take another look at our repository status: `git status`



To push your changes to GitHub, you will use the command:

```sh
git push
```

> When you push, you will be asked to enter your GitHub username and password. If you would like Git to remember your credentials on this computer, you can cache your credentials using:

- Windows: `git config --global credential.helper wincred`