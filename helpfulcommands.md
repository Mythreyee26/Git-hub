 See what git is tracking:

   ```sh
   git status
   ```

1. Create a new, empty directory:

   ```sh
   mkdir images
   ```

1. Move the texture file into the directory with git:

   ```sh
   git mv texture.jpg images/texture.jpg
   ```

### Staging hunks of changes

Crafting atomic commits is an important part of creating a readable and informative history of the project.

1. See what git is tracking:

   ```sh
   git status
   ```

1. Move some parts of some files to the staging area with the `--patch` flag:

   ```sh
   git add -p
   ```

1. Stage the hunk related to the image move: <kbd>y</kbd>
1. Leave the hunk related to the speed change in the working area: <kbd>n</kbd>

?> Wondering what all of those other options are for the hunks? Use <kbd>?</kbd> to see a list of options above the hunk.

`git config --global alias.cm "!git add -A && git commit -m"` could be helpful here. Check out the appendix to see how!

`git diff` allows you to see the difference between any two refs in the repository. The diagram below shows how you can compare the content of your working area, staging, and HEAD (or the most recent commit):

```sh
git diff
git diff --staged
git diff HEAD
git diff --color-words
```

`git diff` will also allow you to compare between branches, commits, and tags by simply typing:

```sh
git diff <REF-1> <REF-2>
git diff main slow-down
git diff origin/main main
git diff 2710 b745
```
