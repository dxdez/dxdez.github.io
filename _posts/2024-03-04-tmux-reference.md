---
layout: post
title:  "TMUX Reference Guide"
date:   2024-03-31 10:26:24 -0500
---

This list contains some essential commands used for TMUX sessions. The origninal source was provided from a document hosted on opensource.com which can be found [here](https://opensource.com/downloads/tmux-cheat-sheet?intcmp=701f20000012ngPAAQ "here")

### Attach and Detach

`tmux new -s [optional-name] [-optional-flag]` - Start new tmux session\
`tmux a -t [name]` - attach Attach to tmux session running in the background\
`Ctrl+B d` Detach from tmux session, leaving it running in the background\
`Ctrl+B &` Exit and quit tmux\
`Ctrl+B ?` List all key bindings (press Q to exit help screen)\

### Window Management
`Ctrl+B ,` - Rename new window\
`Ctrl+B C` - Create new window                \
`Ctrl+B N` - Move to next window              \
`Ctrl+B P` - Move to previous window          \
`Ctrl+B L` - Move to last window              \
`Ctrl+B 0-9` - Move to window by index number \

### Session Management
`Ctrl+B )` - Move to next session\
`Ctrl+B (` - Move to previous session\
`Ctrl+B S` - Open session manager
`Ctrl+B Ctrl+Z` - Suspend session\
`Ctrl+B Ctrl+B [key]` - To execute commands in nested session, press the command twice followed by the desired key\

### Split Window into Panes
`Ctrl+B %` - Vertical split (panes side by side)                   \
`Ctrl+B "` - Horizontal split (one pane below the other)           \
`Ctrl+B O` - Move to other pane                                    \
`Ctrl+B !` - Remove all panes but the current one from the window  \
`Ctrl+B Q` - Display window index numbers                          \
`Ctrl+B Ctrl-Up/Down` - Resize current pane (due north/south)      \
`Ctrl+B Ctrl-Left/Right` - Resize current pane (due west/east)     \

### Multiplex
`Ctrl+B :` - Access tmux command prompt\
`Ctrl+B :setw synchronize-panes on` - Synchronize panes (to send a command to many hosts)\

#### Command Prompt Example
`tmux rename-session [-t current-name] [new-name]` - Renames the session by name, or current session if none provided
`tmux new -s sample -d` - Creates a new session called `sample` and then detaches, it will still run in the background
`tmux ls` - Lists the currently running tmux sessions
`ssh <hostname> -t tmux a` - connect and attach to tmux session via ssh - note, an active session needs to be running

### Additional Commands
`Ctrl+B ,` - Rename current window in session\
`x, y` - Within session manager, x will close a session, y will confirm, you can also close multiple using `t`

### TMUX manpage & additional resources
- Additional documentation for TMUX from the manual page can be found [here](https://man.openbsd.org/OpenBSD-current/man1/tmux.1 "here")
- Information on attaching tmux sessions to ssh connections can be found [here](https://jordanelver.co.uk/blog/2010/11/27/automatically-attaching-to-a-tmux-session-via-ssh/ "here")
- Additional commands and best practices can be found [here](https://www.linuxtrainingacademy.com/tmux-tutorial/#:~:text=The%20simplest%20way%20to%20use%20tmux%20is%20to%20run%20the%20tmux%20command.&text=This%20starts%20a%20new%20tmux,this%20case%20is%20%E2%80%9C0%E2%80%9D. "here") 
- There is also a guide on creating a custom script to help with SSH login [here](https://ostechnix.com/enhancing-ssh-login-with-a-tmux-session-selection-menu/#:~:text=If%20you%20don't%20want,name%20for%20the%20new%20session.&text=After%20typing%20the%20name%20of,to%20the%20new%20tmux%20session. "here")


