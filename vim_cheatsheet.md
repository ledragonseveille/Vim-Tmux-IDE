# A Collection of Notes Regarding Vim Usage

## Ex Commands

`:so %` source the file currently edited (for example, .vimrc)  
`:set rtp?` display paths used by Vim (~/.vim, etc.)  
`:his` list the command history  
`:his /` list the search history  
`:set list` display special characters (tab, EOL, etc.)  
`:set list!` stop displaying special characters  

#### Substitution

`:s/foo/bar/g` find each occurrence of 'foo' in the current line only, and replace it with 'bar'  
`:%s/foo/bar/g` find each occurrence of 'foo' in all lines, and replace it with 'bar'  
`:%s/foo/bar/gc` change each 'foo' to 'bar', but ask for confirmation first  
`:%s/\<foo\>/bar/g` change only whole words exactly matching 'foo' to 'bar'  

#### Buffers

Vim allows us to work with multiple buffers simultaneously.

`:ls` list buffers loaded in memory  
`:bnext` or `:bn` jump to next buffer  
`:bprev` or `:bp` jump to previous buffer  
`:b<num>` jump to buffer <num>

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

Ref : https://www.freecodecamp.org/news/learn-linux-vim-basic-features-19134461ab85/

Workflow:
* Open any number of tabs you wish to work with
* From any tab, enter command mode
* Type `:mksession <session_name>.vim` and hit enter
* Your current session of open tabs will be stored in a file named <session_name>.vim
* To restore a session, close all tabs and Vim
* Either start vim with your session using : `$ vim -S <session_name>.vim` or open Vim with any other file and enter command mode to type: `:source <session_name>.vim` 
* If you change any session tabs (close/open new), you can save that back using : `:mks!` while you are in the session

## Misc

When you need to return temporarily to the shell when editing a file, instead of exiting vim, just do `CTRL+z` (in command mode), then `fg` when you want to go back into vim! :-)

## Resources

### Web sites

[Vi improved](https://www.vi-improved.org)

### Videos

[Vim as an IDE](https://www.youtube.com/watch?v=Gs1VDYnS-Ac)  
[How to stop using Vim like a pig](https://www.youtube.com/watch?v=D2B3YI_d6HA)  
[How to do 90% of what plugins do (with just Vim)](https://www.youtube.com/watch?v=XA2WjJbmmoM&t=3s)

