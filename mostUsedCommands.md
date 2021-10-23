# Git Aliases

- git c = commit -am
- git amend = commit --amend --all --no-edit
- git undocommit = reset HEAD~
- git hreset = reset --hard
- git unstage = reset --soft HEAD
- git diff
- git lg = log
- git diffbranch = !"git diff $(git merge-base HEAD origin/master)"

- git # Show the diff between the latest commit and the current state
  d = !"git diff-index --quiet HEAD -- || clear; git --no-pager diff --patch-with-stat"

- git go = creates new branch and/or go to branch
- git aliases
- git contributors

# CLI

- p = project directory
- cz = open zshrc
- net = check if internet is working
- ram <software> = check how much ram it consumes
- update-mac
- mg = Create a new directory and enter it
- whois = whois a domain or a URL
- ff <thing> = search a folder

# VSCode Shortcuts
  
## Move between tabs:
  - Control + Tab (move to the right) or Control + Shift + Tab (move to the left)
