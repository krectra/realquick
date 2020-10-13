- Split pane vertically
  - `Ctrl B + Shift %`
  
- Split pane horizontally
  - `Ctrl B + Shift "`

- Close pane
  - `Ctrl B + x`


# Shared session
## Create session
- tmux -S /tmp/shareds new -s shared

## Attach session
- tmux -S /tmp/shareds attach -t shared

### Reference
https://www.howtoforge.com/sharing-terminal-sessions-with-tmux-and-screen
