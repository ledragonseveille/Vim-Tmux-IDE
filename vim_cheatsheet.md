# A Collection of Notes Regarding Vim Usage

## Ex Commands

`:so %` source the file currently edited (for example, .vimrc)  
`:set rtp?` display paths used by Vim (~/.vim, etc.)  
`:ls` list buffers loaded in memory  
`:his` list the command history  
`:his /` list the search history  
`:set list` display special characters (tab, EOL, etc.)  
`:set list!` stop displaying special characters  

## Tabs

`:tabedit <file>` open <file> in a new tab  
`gt` go to next tab  
`gT` go to previous tab  
`{i}gt` go to the tab with index {i}  
`:tabfirst`  
`:tablast`  
`:tabs` list all the open tabs  
`:tabclose` close a single tab  
`:tabonly` close all tabs except the current one  
