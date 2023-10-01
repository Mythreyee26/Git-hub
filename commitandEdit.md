### COMMITS:

git commit -m "Version1"
git commit -a -m ""
git commit -am ""

### REMOVE:
rm
git rm file.txt 

git rm *.txt 

git rm -h 

git rm --cached -r bin/ (to remove only from the index )

rm -rf .git (removes everything in the repo)

### See what git is tracking:

   ```sh
   git status
   ```

### Create a new, empty directory:

   ```sh
   mkdir images
   ```

### Move the texture file into the directory with git:

   ```sh
   git mv texture.jpg images/texture.jpg
   ```

### Move some parts of some files to the staging area with the `--patch` flag:

   ```sh
   git add -p
   ```
### Alias

`git config --global alias.cam "!git add -A && git commit -m"` 

```sh
git cam
``` 

`git config --global alias.lol "log --oneline --graph --decorate --all"`

```sh
git lol
``` 

`git config --global alias .s "status"`
```sh
git s
``` 
`git config --global alias .cm "commit -m"`
```sh
git cm
``` 
`git config --global alias.ec "config --global -e"`
```sh
git ec
``` 
`git config --global alias.ch "checkout"`
```sh
git ch
``` 
`git config --global alias.cob "checkout -b"`
```sh
git cob
``` 
`git config --global alias.s "status -s"`
```sh
git s
``` 
