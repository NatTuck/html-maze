
Readme for HTML Maze

## Enter The Maze

[Enter The Maze](./maze/)

## Setup:

- Install npm: `sudo apt install pandoc`

## Convert a MD file to HTML

To convert index.md (from src dir) to index.html (in maze dir):

```
pandoc -o maze/index.html src/index.md
```

## Setup a Git Repostiory

In our project directory with stuff in it: `git init .`

(if it complains about defaultBranch, do `git config --global init.defaultBranch main`)

```
git status
git add -A .
git commit -a -m 'maze'
```
