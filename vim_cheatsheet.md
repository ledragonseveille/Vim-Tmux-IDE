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

## Vim Session

Workflow:
* Open any number of tabs you wish to work with
* From any tab, enter command mode
* Type `:mksession <session_name>.vim` and hit enter
* Your current session of open tabs will be stored in a file named <session_name>.vim
* To restore a session, close all tabs and Vim
* Either start vim with your session using : `$ vim -S <session_name>.vim` or open Vim with any other file and enter command mode to type: `:source <session_name>.vim` 
* If you change any session tabs (close/open new), you can save that back using : `:mks!` while you are in the session
