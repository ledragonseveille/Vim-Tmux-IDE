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
