
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

## Setup an SSH key

```
ssh-keygen
```

Then press enter three times for blank responses.

```
cat ~/.ssh/id_ed25519.pub
```

Copy the thing that looks kind of like:

```
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIL/lzNEzueQ5PraDma4brKJ3Xq7N3I9yvzNKbrBY+Vfq rbl@psu-robotics-noble-1

```

## On Github

- Create new repository, probably with the same name as the project directory.
- Settings (for the new repository), deploy keys, add deploy key, paste in big box;
check "Allow write access"

Back on Code, make sure SSH is selected, and follow the directions to push
an existing repository from the command line.

Once you push, the stuff should be in your repository.

Finally, set up Github Pages

- Settings (for the repository), Pages, Deploy from a branch, called main, save.

It'll take a second, but eventually the Pages settings screen will say
"Your site is live at" and give a link.


## Finally, security cleanup

- You just created an SSH key that's authorized to make changes to a repository
on your Github account.
- If you did that on a lab computer, you probably want to delete it from either
the lab computer or the github repo (or both) once you're done.
- Delete from lab computer with `rm ~/.ssh/id_ed25519`
- Delete from the Github repo by clicking back to settings, deploy keys,
and hitting the delete butto
## Finally, security cleanup

- You just created an SSH key that's authorized to make changes to a repository
on your Github account.
- If you did that on a lab computer, you probably want to delete it from either
the lab computer or the github repo (or both) once you're done.
- Delete from lab computer with `rm ~/.ssh/id_ed25519`
- Delete from the Github repo by clicking back to settings, deploy keys,
and hitting the delete button.
