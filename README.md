# tmux.conf
## Installation
Sym link a file called ~/.tmux.conf to the repos conf then restart.
(File does not need be created before sym link can be attempted).
`ln -s ~/tmux.conf/tmux.conf ~/.tmux.conf`
## Configure TMUX to launch by default
```
if command -v tmux &> /dev/null && [ -z "$TMUX" ]; then
    tmux attach -t default || tmux new -s default
fi
```
