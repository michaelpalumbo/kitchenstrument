
Making changes to an existing repository:
1. Open Terminal.app (I use iTerm2.app, its prettier)
2. Point the terminal to the local repository you want to work on:
```shell
cd /path/to/repository
```
Some commands:
3. check the status of the repository
```shell
git status
```
4. if there are uncommitted changes/files:
```shell
// stage a single file
git add <filename>
// stage all files at once
git add .
```
5. commit the staged files
```shell
git commit -m "message about how fun this is"
```
- make sure all files have been staged and committed before doing next step (repeat steps 4 and 5)

6. check to see if someone else made changes to the repo since your last pull
```shell
git pull
```
If you get a merge conflict, the annoying Vim editor will appear. Most of the time you can type 
```shell
:q!
```
to save and quit a merge message. 
Either way once the pull is resolved, you can *push* your changes to the cloud
```shell
git push
```
