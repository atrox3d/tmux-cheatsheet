# tmux shortcuts & cheatsheet

start new:

    tmux

start new with session name:

    tmux new -s myname

attach:

    tmux a  #  (or at, or attach)

attach to named:

    tmux a -t myname

list sessions:

    tmux ls

kill session:

    tmux kill-session -t myname

In tmux, hit the prefix `ctrl+b` (my modified prefix is ctrl+a) and then:

## Sessions

    :new<CR>  new session
    s  list sessions
    $  name session

## Windows (tabs)

    c  new window
    w  list windows
    f  find window
    ,  name window
    &  kill window

## Panes (splits)

    %  horizontal split
    "  vertical split
    
    o  swap panes
    q  show pane numbers
    x  kill pane
    +  break pane into window (e.g. to select text by mouse to copy)
    -  restore pane from window
    ⍽  space - toggle between layouts

## Misc

    d  detach
    t  big clock
    ?  list shortcuts
    :  prompt

Resources:

* [tmux: Productive Mouse-Free Development](http://pragprog.com/book/bhtmux/tmux)
* [How to reorder windows](http://superuser.com/questions/343572/tmux-how-do-i-reorder-my-windows)
* [cheat sheet](http://cheat.errtheblog.com/s/tmux/)

## Configurations Options:

    #mouse support - set to on if you want to use the mouse
    * setw -g mode-mouse off
    * set -g mouse-select-pane off
    * set -g mouse-resize-pane off
    * set -g mouse-select-window off

#Set the default terminal mode to 256color mode
set -g default-terminal "screen-256color"

Notes:

* 

TODO:

* 