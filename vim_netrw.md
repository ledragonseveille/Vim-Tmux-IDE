# Netrw

## Invoking netrw

Invoking netrw can be achieved in three ways:

* `:Explore` opens netrw in the current window
* `:Sexplore` opens netrw in a horizontal split
* `:Vexplore` opens netrw in a vertical split

## Changing the directory view in netrw

With the directory browser open, hit `i` to cycle through the view types.

There are four different view types: thin, long, wide and tree. 

A preferred view type can be made permanent by setting it in a `.vimrc` file:

```let g:netrw_liststyle = 4```

## Removing the banner

To remove it temporarily press `I`. 

To remove it permanently add the following to your `.vimrc`:

```let g:netrw_banner = 0```

## sorting files

Press `s` to sort files by name, time, or size.

## Quick reference: maps

* `<CR>`: enter a directory or read a file
* `-`: go up one directory
* `t`: enter the file/directory under the cursor in a new tab


## .vimrc example

```
let g:netrw_banner = 0
let g:netrw_liststyle = 3
let g:netrw_browse_split = 4
let g:netrw_altv = 1
let g:netrw_winsize = 25
augroup ProjectDrawer
  autocmd!
  autocmd VimEnter * :Vexplore
augroup END
```
