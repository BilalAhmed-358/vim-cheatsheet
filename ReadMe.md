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
| `:e filename` | Open a file |
| `:sp filename` | Open file in a horizontal split |
| `:vsp filename` | Open file in a vertical split |

## Modes

| Command | Description |
|---------|-------------|
| `Esc` | Normal mode. Default starting mode. |
| `i` | Insert mode before cursor. Esc to normal mode. |
| `a` | Insert mode after cursor. Esc to normal mode. |
| `v` | Visual mode. Esc to normal mode. |
| `V` | Visual Line mode. Esc to normal mode. |
| `:` | Command-line mode. Esc to normal mode. |

## Getting Around

| Command | Description |
|---------|-------------|
| `h` `j` `k` `l` | Left, Down, Up, Right |
| `w` | Forward a word |
| `b` | Backwards a word |
| `e` | Jump to end of word |
| `0` | Beginning of line |
| `$` | End of line |
| `gg` | Top of file |
| `G` | Bottom of file |
| `:{n}` or `{n}G` | Jump to line number n (e.g. `:42` or `42G`) |
| `Ctrl+d` | Half-page down |
| `Ctrl+u` | Half-page up |
| `%` | Jump to matching bracket |

## Line Numbers

| Command | Description |
|---------|-------------|
| `:set number` | Show absolute line numbers |
| `:set relativenumber` | Show relative line numbers |
| `:set number relativenumber` | Show absolute on current line, relative elsewhere |
| `:set nonumber` | Hide line numbers |
| `:set norelativenumber` | Hide relative line numbers |

To persist line numbers, add to `~/.vimrc`:
```
set number
set relativenumber
```

## Making Changes

| Command | Description |
|---------|-------------|
| `i` | Insert mode before cursor |
| `a` | Insert mode after cursor |
| `o` | Insert new line below |
| `O` | Insert new line above |
| `I` | Insert at beginning of line |
| `A` | Insert (append) at end of line |
| `x` | Delete character under cursor |
| `dd` | Delete line |
| `2dd` | Delete two lines |
| `dw` | Delete word |
| `d$` | Delete to end of line |
| `5x` | Delete 5 characters |
| `dG` | Delete from cursor to end of file |
| `dgg` | Delete from cursor to beginning of file |
| `yy` | Yank (copy) a line |
| `yw` | Copy word |
| `p` | Paste after cursor |
| `P` | Paste before cursor |
| `u` | Undo |
| `Ctrl+r` | Redo |
| `ciw` | Change inner word (delete word and enter Insert mode) |
| `ci"` | Change inside quotes |
| `>>` | Indent line |
| `<<` | Unindent line |
| `.` | Repeat last change |

## Selecting Text

| Command | Description |
|---------|-------------|
| `v` | Character-wise selection |
| `V` | Line-wise selection |
| `Ctrl+v` | Block selection |
| Arrow keys | Highlight text in Visual mode |
| `y` | Yank (copy) selection |
| `c` | Change (cut) selection |
| `d` | Delete selection |
| `p` | Paste selection |
| `>` | Indent selection |
| `<` | Unindent selection |
| `Esc` | Return to Normal mode |

## Search, Replace & Undo

| Command | Description |
|---------|-------------|
| `/pattern` | Search forward |
| `?pattern` | Search backward |
| `n` | Next match |
| `N` | Previous match |
| `:%s/old/new/g` | Replace all occurrences in file |
| `:%s/old/new/gc` | Replace all with confirmation |
| `:s/old/new/g` | Replace all in current line |
| `u` | Undo |
| `Ctrl+r` | Redo |
| `:set paste` | Disable auto-indent upon paste |
| `:set nopaste` | Re-enable auto-indent upon paste |
