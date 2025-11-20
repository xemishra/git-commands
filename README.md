<h2 align='center'> A simple, well-organized reference of essential Git commands for quick learning and everyday use. </h2>
<h1 align='center'> Git-Commands List</h1>

## 1. Configuration Commands - Commands used to set user details, preferences, and Git behavior.
```bash
git config --global user.name "Your Name"
```
```bash
git config --global user.email "your@email.com"
```
```bash
git config --list
```
```bash
git config --global core.editor nano
```
```bash
git config --global init.defaultBranch main
```
## 2. Repository Setup - Commands for creating, cloning, and initializing repositories.
```bash
git init
```
```bash
git init --bare
```
```bash
git clone <url>
```
```bash
git clone --branch <branch> <url>
```
## 3. File Tracking & Staging - Commands for selecting and preparing files before committing.
```bash
git status
```
```bash
git add <file>
```
```bash
git add .
```
```bash
git add -p
```
```bash
git add -A
```
## 4. Commit Commands - Commands for recording changes into the Git history.
```bash
git commit -m "message"
```
```bash
git commit -a -m "message"
```
```bash
git commit --amend
```
```bash
git commit --amend -m "new message"
```
## 5. Branching - Commands for creating, listing, renaming, and deleting branches.
```bash
git branch
```
```bash
git branch <name>
```
```bash
git branch -d <name>
```
```bash
git branch -D <name>
```
```bash
git branch -m <old> <new>
```
```bash
git branch -a
```
```bash
git branch -r
```
## 6. Checkout / Switch - Commands used to move between branches or restore file states.
```bash
git checkout <branch>
```
```bash
git checkout -b <branch>
```
```bash
git switch <branch>
```
```bash
git switch -c <branch>
```
```bash
git checkout -- <file>
```
## 7. Merging - Commands for combining changes from different branches.
```bash
git merge <branch>
```
```bash
git merge --no-ff <branch>
```
```bash
git merge --abort
```
## 8. Rebase - Commands for rewriting commit history and applying commits over another base.
```bash
git rebase <branch>
```
```bash
git rebase -i <branch>
```
```bash
git rebase --continue
```
```bash
git rebase --abort
```
```bash
git rebase --skip
```
## 9. Remote Commands - Commands for managing remote repositories and connections.
```bash
git remote
```
```bash
git remote -v
```
```bash
git remote add origin <url>
```
```bash
git remote remove <name>
```
```bash
git remote rename <old> <new>
```
## 10. Push Commands - Commands for managing remote repositories and connections.
```bash
git push
```
```bash
git push -u origin main
```
```bash
git push --force
```
```bash
git push --force-with-lease
```
```bash
git push origin --delete <branch>
```
## 11. Pull & Fetch - Commands for retrieving updates from remote repositories.
```bash
git pull
```
```bash
git pull origin <branch>
```
```bash
git pull --rebase
```
```bash
git fetch
```
```bash
git fetch --all
```
## 12. Stash Commands - Commands for temporarily saving uncommitted changes.
```bash
git stash
```
```bash
git stash save "message"
```
```bash
git stash list
```
```bash
git stash apply
```
```bash
git stash pop
```
```bash
git stash drop
```
```bash
git stash clear
```
## 13. Log & History - Commands for viewing commit history and change records.
```bash
git log
```
```bash
git log --oneline
```
```bash
git log --graph
```
```bash
git log --stat
```
```bash
git log -p
```
## 14. Diff Commands - Commands for comparing file changes between commits, branches, or workspaces.
```bash
git diff
```
```bash
git diff --staged
```
```bash
git diff <branch1> <branch2>
```
```bash
git diff <commit1> <commit2>
```
## 15. Tagging - Commands for marking specific commits with version tags.
```bash
git tag
```
```bash
git tag <tagname>
```
```bash
git tag -a <tagname> -m "message"
```
```bash
git push origin <tagname>
```
```bash
git push --tags
```
```bash
git tag -d <tagname>
```
## 16. Reset Commands - Commands for undoing changes or moving the HEAD to another commit.
```bash
git reset <file>
```
```bash
git reset --soft <commit>
```
```bash
git reset --mixed <commit>
```
```bash
git reset --hard <commit>
```
## 17. Restore Commands - Commands for restoring working directory or staged files to previous states.
```bash
git restore <file>
```
```bash
git restore --staged <file>
```
```bash
git restore --source <commit> <file>
```
## 18. Clean Workspace - Commands for removing untracked files or directories.
```bash
git clean -n
```
```bash
git clean -f
```
```bash
git clean -fd
```
```bash
git clean -fx
```
## 19. Cherry-Pick - Commands for applying specific commits on top of the current branch.
```bash
git cherry-pick <commit>
```
```bash
git cherry-pick --continue
```
```bash
git cherry-pick --abort
```
## 20. Submodule Commands - Commands for managing repositories embedded inside another repository.
```bash
git submodule add <url>
```
```bash
git submodule init
```
```bash
git submodule update
```
```bash
git submodule update --remote
```
```bash
git submodule deinit -f .
```
## 21. Bisect (Debugging) - Commands for finding the commit that introduced a bug.
```bash
git bisect start
```
```bash
git bisect good <commit>
```
```bash
git bisect bad <commit>
```
```bash
git bisect reset
```
## 22. Archive & Export - Commands for packaging a repository or commit into an archive.
```bash
git archive --format zip --output file.zip HEAD
```
```bash
git archive --format tar HEAD
```
## 23. Grep (Search) - Commands for searching text patterns inside tracked files.
```bash
git grep <text>
```
```bash
git grep -n <text>
```
```bash
git grep -p <pattern>
```
## 24. Blame & Annotate - Commands for showing which commit modified each line of a file.
```bash
git blame <file>
```
```bash
git blame -L <start>,<end> <file>
```
## 25. Reflog - Commands for viewing history of HEAD movements.
```bash
git reflog
```
```bash
git reflog expire
```
```bash
git reflog delete
```
## 26. Worktree - Commands for managing multiple working directories attached to one repo.
```bash
git worktree add <path> <branch>
```
```bash
git worktree list
```
```bash
git worktree remove <path>
```
## 27. Apply Patch - Commands for applying or generating patch files.
```bash
git apply <patch>
```
```bash
git apply --check <patch>
```
## 28. Format Patch - Commands for applying or generating patch files.
```bash
git format-patch HEAD~1
```
```bash
git format-patch --cover-letter
```
## 29. Sparse Checkout - Commands for checking out only specific folders of a repo.
```bash
git sparse-checkout init
```
```bash
git sparse-checkout set <folder>
```
## 30. Maintenance Commands - Commands for repository health, cleanup, and optimization.
```bash
git gc
```
```bash
git fsck
```
```bash
git prune
```
### Download PDF: [Click Here](https://github.com/xemishra/git-commands/blob/main/gitCommands.pdf) 

### Contact: [Click Here](https://mishraxe.t.me)

<div align="center">
  <h2>Made with ❤️ By <a href="https://github.com/xemishra">Shivanand Mishra</a></h2>
</div>
