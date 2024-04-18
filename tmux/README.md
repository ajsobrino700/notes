# tmux

The first thing is that, there is some resources on the internet very interesting. For example [cheat sheet](https://tmuxcheatsheet.com) or tutorial on youtube.

Tmux is a very interesting tool for command line, we can have a multiplexer terminal. Also we can have a panel, split the screen, windows, sessions and customatize the command and the view with a settings file.

We start a session with the next command
```zsh
 tmux
```
Inside of the session we have a complete terminal. We can exit to the session with **exit** or detach the session without close with **ctr+b|d**.
If we are outside of session we can do several actions:
```zsh
    # list sessions.
    tmux list-sessions
    tmux ls
    # Inside to session opened.
    tmux attach \# Open the session most recent.
```

Previously we speak about the feature to split the screen in several terminals, the name of those terminals is *panes*.
It is possible to do split vertical or horizontal. This split will be from the current *pane*, so it is important to have the control of the focussing *pane*.
We can do a vertical split with **ctr+b | "** and the horizontal split with **ctr+b | %**, finally we can move the focus with the same prefix and the arrow of the keyboard.
We can change the size of our pane, it is very easy, we use the prefix and **alt+arrow** depends of the direction of the arrow the pane will resize in this direction.

Other very important concept is *window*. We can create a window when we are inside of the tmux session, we execute the follow command
```zsh
 tmux new-window
```
We may view the information about the windows in the below bar. Also we need to move between windows. This action will do with the prefix **ctr+b** and *p* for previous and *n* for next window.
The way to kill the window is prefix and **&**.
Finally to finish this subject we are going to change the name of the window. We need to press *prefix* and *,* and we rename the current window. Algo we can change name of the window though comman
```zsh
    tmux rename-window <nre-name>
```

The next topic is manage the sessions in tmux. We can create a new session only with the command *tmux*. In addition we can choose which session we want to open with the next command
```zsh
    tmux attacth -t <name> 
    tmux a -t <name>
```
The second option is the same but with the short way. Moroever we can rename the session vert easy with a command
```zsh
    tmux rename-session <name>
```
The previous command, it changes the current tmux session name. We can change the name with a short way: *prefix* and *\$*.
A command very important and interesting if you are working with session is *prefix* and *s*. We get a list of the session and we can change between the sessions that we have opened in this moment.
Finally if we want to move very easy in the sessions we can use *prefix* and *(* or *)*, we change to the next or previous session.

By other hand, something so much important is how can I close a session or panel? It is very simple, the command **exit**. Other trick relation with that is press *ctr+d**, although it is not a shortcut of tmux is a terminal trick.

The last topic in this notes is the customize command and stetic and other similar things.

The file with the settings of tmux is **.tmux.conf**. We will add the configuration that we want for our customize. We can override the default settings and add some new configuration.

The first interesting setting is activate the mouse mood
```zsh
    set -g mouse on
```
