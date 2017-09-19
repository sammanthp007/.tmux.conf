# .tmux.conf
My tmux configuration.

Defaults for zsh shell. If you use bash, then change the first config in [tmux config file](.tmux.conf) to /bin/bash

## Table of Content
- [To use](#to-use)
- [Features](#features)
- [Extras](#extras)
  - [For Mac terminal](#for-mac-terminal)

## To use
1. Install tmux in your system: 
```
# For Ubuntu/debian
sudo apt install tmux
# For Arch
sudo pacman -S tmux
```
2. Download and set up the dotfile here
```
git clone https://github.com/sammanthp007/.tmux.conf.git tmux && mv tmux/.tmux.conf ~/.tmux.conf && rm -rf tmux
```

## Features 

### Triggering tmux
```
<c-s> instead of default <c-b> for convenience
```

### For switching
```
# to move between panes
<c-h>
<c-j>
<c-k>
<c-l>
```

### Split window horizontally
```
<c-a> + |
```
### Split window vertically
```
<c-a> + -
```

### Move splits
```
<c-a> + {
<c-a> + }
```

### Resizing Panes
```
<c-b> : resize-pane -D (Resizes the current pane down)
<c-b> : resize-pane -U (Resizes the current pane upward)
<c-b> : resize-pane -L (Resizes the current pane left)
<c-b> : resize-pane -R (Resizes the current pane right)
<c-b> : resize-pane -D 20 (Resizes the current pane down by 20 cells)
<c-b> : resize-pane -U 20 (Resizes the current pane upward by 20 cells)
<c-b> : resize-pane -L 20 (Resizes the current pane left by 20 cells)
<c-b> : resize-pane -R 20 (Resizes the current pane right by 20 cells)
<c-b> : resize-pane -t 2 20 (Resizes the pane with the id of 2 down by 20 cells)
<c-b> : resize-pane -t -L 20 (Resizes the pane with the id of 2 left by 20 cells)
```

## Extras
### For Mac terminal
Be able to use `pbcopy` and `pbpaste`
```
brew install reattach-to-user-namespace
 
 # and add the following to ~/.tmux.conf
 set-option -g default-command "reattach-to-user-namespace -l zsh"
 ```
