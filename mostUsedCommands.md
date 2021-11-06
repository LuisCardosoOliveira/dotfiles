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
  
## Move between lines:
  - Fn + Left arrow = move to the begin of the line
  - Fn + Rigt arrow = move to the end of the line
  - Fn + Left arrow + Shitft = Selects from current cursor position to start of line
  - Fn + right arrow + Shitft = Selects from current cursor position to end of line
  - Fn + CMD + Arrow up or down = move fast between file
  - CMD + arrow down/up = move to end or begin of the file
  - Option + arrow right/left = move cursor to the end/begin of the word
  - Option + Shitft + Down = duplicates line
  - Shit + arrow up = Expand selection
  - Control + Shift + arrow-right = select all elements within the scope
  
  
  ## General shortcuts: 
  - CMD + B = close/open sidebar
  - CMD + D = select word (or words) where the cursor is
  - CMD + 1,2,3.etc = split editor
  - CMD + L = select the current line where cursor is
  - Option + Click = Multi cursor selection
  - Control + R in the terminal = search for previous commands

  
  
