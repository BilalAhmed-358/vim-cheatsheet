# Vim Cheatsheet

## Opening & Saving

| Command | Description |
|---------|-------------|
| `vim <filename>` | Open a file in Vim |
| `:w` | Save a file |
| `:q` | Quit a file |
| `:wq` | Save and quit |
| `:q!` | Quit without saving |
| `ZZ` | Save (if modified) and exit |
| `:w <filename>` | Save a copy as filename |

## Modes

| Command | Description |
|---------|-------------|
| `Esc` | Normal mode. Default starting mode. |
| `i` | Insert mode. Esc to normal mode. |
| `v` | Visual mode. Esc to normal mode. |
| `:` | Command-line mode. Esc to normal mode. |

## Getting Around

| Command | Description |
|---------|-------------|
| Arrow keys | Move around (or `h`,`j`,`k`,`l` — left, down, up, right) |
| `$` | End of line |
| `0` | Beginning of line (this is a 'zero', not an 'o') |
| `Ctrl + u` | Half-page up |
| `Ctrl + d` | Half-page down |
| `b` | Backwards a word |
| `w` | Forward a word |
| `G` | Bottom of file |
| `gg` | Top of file (or `1G`) |
| `:set number` | Display line numbering |
| `:set nonumber` | Hide line numbering |
| `:5` | Go to line 5 |

## Making Changes

| Command | Description |
|---------|-------------|
| `i` | Insert mode. Esc to normal mode. |
| `o` | Insert new line below |
| `O` | Insert new line above |
| `I` | Insert at beginning of line |
| `A` | Insert (append) at end of line |
| `x` | Delete character |
| `dd` | Delete line |
| `2dd` | Delete two lines |
| `5x` | Delete 5 characters |
| `dG` | Delete from cursor to end of file |
| `d$` | Delete from cursor to end of line |
| `dgg` | Delete from cursor to beginning of file |
| `yy` | Yank (copy) a line |

## Selecting Text

| Command | Description |
|---------|-------------|
| `v` | Enter Visual mode |
| Arrow keys | Highlight text in Visual mode |
| `y` | Yank (copy) selection |
| `c` | Change (cut) selection |
| `d` | Delete selection |
| `p` | Paste selection. Esc to enter normal mode to paste. |
| `Esc` | Enter normal mode |

## Search, Replace & Undo

| Command | Description |
|---------|-------------|
| `u` | Undo (from normal mode) |
| `Ctrl + r` | Redo (from normal mode) |
| `/searchterm` | Search for searchterm. Add `\c` for case insensitive. |
| `n` | Next instance of searchterm |
| `N` | Previous instance of searchterm |
| `:%s/replaceme/withme/g` | Replace "replaceme" with "withme" in the entire file |
| `:%s/replaceme/withme/gc` | Replace "replaceme" with "withme" and prompt |
| `:set paste` | Disable auto-indent upon paste |
| `:set nopaste` | Re-enable auto-indent upon paste |
| `?searchterm` | Search backwards in file for searchterm |
| `.` | Repeat last change |
