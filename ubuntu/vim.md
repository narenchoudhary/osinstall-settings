# Vim

##  Auto Indentation, Tap Width, Tab to Spaces, Line Numbers

    filetype plugin indent on
    " show existing tab with 4 spaces width
     set tabstop=4
    " when indenting with '>', use 4 spaces width
    set shiftwidth=4
    " On pressing tab, insert 4 spaces
    set expandtab
    set number
    set colorcolumn=80                                                                                                                           
    set cursorline                                                                  
    set cursorcolumn                                                                
    let g:airline_powerline_fonts = 1 

## Stop using arrows

Put these lines in `~/.vimrc`:

    noremap <Up> <NOP>
    noremap <Down> <NOP>
    noremap <Left> <NOP>
    noremap <Right> <NOP>

## To stop vim from hanging when ctrl+S is pressed accidently

One time solution:  
Press CTRL+Q

Better solution:  
Append `stty -ixon` in a startup script.

Source: https://unix.stackexchange.com/a/12108

