# A Collection of Notes Regarding Tmux Usage

Default prefix key: \<Ctrl-b\>

**NOTE**: PREFIX will replace \<Ctrl-b\> in the rest of the document.

## Session

`PREFIX`+`d` to detach current session  
`tmux attach` to attach the session  
`PREFIX`+`$` to rename a session  

## Window

`PREFIX`+`c` to create a new window  
`PREFIX`+`,` to rename a window  

#### Navigation

`PREFIX`+`n` to jump to next window  
`PREFIX`+`p` to jump to previous window  
`PREFIX`+`1` or `2` (etc.) to navigate via window's index  
`PREFIX`+`'` to prompt for a window index  
`PREFIX`+`f` to forward to a window with a match of a text string  
`PREFIX`+`l` to bring up the last selected window  
`PREFIX`+`w` to list the current windows  

## Pane

`PREFIX`+`x` to kill panes  
`PREFIX`+`%` to split window horizontally  
`PREFIX`+`"` to split window vertically  

#### Navigation

`PREFIX`+`;` to move to the previously active pane  
`PREFIX`+`UP` or `DOWN` or `RIGHT` or `LEFT` to change to the pane above, below, to the right or to the left of the current pane  
`PREFIX`+`o` to select the next pane in the current window  
`PREFIX` + `PAGEUP` to be able to scroll the pane history (then PAGEUP or PAGEDOWN, and ESC to quit the mode)  
