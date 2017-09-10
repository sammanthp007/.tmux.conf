# .tmux.conf
My tmux configuration.

Defaults for zsh shell. If you use bash, then change the first config in [tmux config file](.tmux.conf) to /bin/bash

## To use
1. Install tmux in your system
2. Download the .tmux.conf file
3. Save it as `~/.tmux.conf`
4. You are good to go

## Some custom key mappings I use 

### Triggering tmux
```
<c-a> instead of default <c-b> for convenience
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
