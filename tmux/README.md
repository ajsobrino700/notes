# tmux

Tmux is a very interesting tool for command line, we can have a multiplexer terminal. Also we can have a panel, split the screen, windows, sessions and customatize the command and the view with a settings file.

We start a session with the next command
```zsh
 tmux
```
Inside of the session we have a complete terminal. We can exit to the session with **exit** or detach the session without close with **ctr+b|d**.
If we are outside of session we can do several actions:
```zsh
    \# list sessions.
    tmux list-sessions
    tmux ls
    \# Inside to session opened.
    tmux attach \# Open the session most recent.
```
