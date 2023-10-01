mkdir logs 
echo hello > logs/dev.log 
git status 


mkdir bin 
echo Queen > bin/add.bin 
git status 
git add .
git commit -m "Add bin" 


echo hiiii > .gitignore 
code .gitignore 
(Opens the IDE )

git add .gitignore 
git commit -m "add git ignore"


git ls-files 

git rm --cached -r bin/
git ls-files 
 
git status 
git commit -m "Remove"

echo test >bin/app.bin 
ls 

DIFF:
git diff --staged 
git diff 
git status -s 

git config --global diff.vscode 
git config --global difftool.vscode.cmd "code --wait --diff $LOCAL $REMOTE"
git config --global -e 

git log 
git log --oneline 
git log --oneline --reverse 
git show HEAD
git show HEAD~1


git ls-tree 
git ls-tree HEAD~1

git clean 
git clean -h
git clean -fd

### Diff

`git diff` 
allows you to see the difference between any two refs in the repository. 

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

