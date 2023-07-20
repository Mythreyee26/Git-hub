git config --list
git config --global --list
git config --global user.name "First-name Surname"
git config --global user.email "you@email.com"
git config --global --unset <property_name>


The instructions for this exercise use the `--global` flag when identifying your `user.name` and `user.email` configuration settings. If you are currently using a computer without a private, personal account, don't apply the `--global` flag. This way, the settings will only be stored in our assignment repository. If you work in another repository on this same computer, you will need to set these configuration options again.

> For example:
>
> ```sh
> git config user.email "you@email.com"

### Configuring autocrlf


//for Windows users
git config --global core.autocrlf true

> Memory Tip: `autocrlf` stands for auto carriage return line feed.


### Using Markdown

GitHub uses a syntax called **Markdown** to help you add basic text formatting to Issues, Pull Requests, and files with the `.md` extension.


### Using Git log

When you clone a repository, you receive the history of all the commits made in that repository. The log command allows us to view that history on our local machine.

Let's take a look at some option switches you can use to customize your view of the project history. You can find these options, and many more, on [git-scm.com](https://git-scm.com/docs/git-log). _(Note: `--graph` is default on most Git Bash for Windows terminals.)_

git log
git log --oneline
git log --oneline --graph
git log --oneline --graph --decorate
git log --oneline --graph --decorate --all
git log --stat
git log --patch



### Original command to alias

```sh
git log --oneline --graph --decorate --all
```

### Creating the alias

```sh
git config --global alias.lol "log --oneline --graph --decorate --all"
```

### Using the alias

```sh
git lol
```



Initialize the revert: `git revert <SHA>`
1. Type a commit message.
1. Push your changes to GitHub


Create a new directory and initialize it as a git repository: `git init practice-repo`
1. CD into your new repository: `cd practice-repo`
1. Create an empty new file named `README.md`:
   - Bash: `touch README.md`

   `git commit --amend` allows us to make changes to the commit that HEAD is currently pointing to. Two of the most common uses are:

- Re-writing commit messages
- Adding files to the commit


 In your Terminal or Git Bash, `cd` to a repository of interest and create a `.gitignore` file:

   ```sh
   touch .gitignore
   ```

   For Windows users who are not using a bash-based terminal:

   ```sh
   echo >> .gitignore
   ```

   1. To share the gitignore rules with other users who clone the repository, commit the `.gitignore` file to your repository.

   ```sh
   git add .gitignore
   git commit -m "add gitignore file"
   ```

   
1. Configure `git` to use this file:

    For Windows Users:

   ```sh
   git config --global core.excludesfile %USERPROFILE%\.gitignore_global
   ```