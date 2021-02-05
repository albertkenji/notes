## Tmux commands and config

> **tmux** is a terminal multiplexer. It lets you use a single enviorment to launch multiple terminals, or windows, each running its own process or program.  

- **Hierarchy**: *session* - *window* - *pane*

## Basic  

- **New Session**

```
tmux new -s <name of session>
```

- **List Sessions**

```
tmux ls
```

- **Attach Session**

```
tmux attach -t <name of session>
```

- **Killing Session**

```
tmux kill-session -t <name of session>
```

- **Command Prefix** - default: <ctrl+b>

* prefix + d - detach session
* prefix + t - large clock on the screen
* prefix + c - create new window
* prefix + , - rename window
* prefix + w - disply visual menu of windows
* prefix + & - kill window (exit)
* prefix + 0 .. 9 - moves to next window

## Plugin Install

- [Tmux Plugin Manager](https://github.com/tmux-plugins/tpm)

* prefix + I

## Manage and restore tmux sessions: Persists tmux environment across system restarts.

- [Plugin Tmux Resurrect](https://github.com/tmux-plugins/tmux-resurrect)

* prefix + <ctrl+s> - save session
* prefix + <ctrl+r> - restore session
