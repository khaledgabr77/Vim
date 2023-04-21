---
marp: true
theme: custom-theme
author: Khaled Gabr

---

# VIM

---
Vim has multiple operating modes:

- `Normal`: for moving around a file and making edits `<ESC>`
- `Insert`: for inserting text `<i>`
- `Replace`: for replacing text `<R>`
- `Visual` (plain <`v`>, line `<V>`, or block `<ctrl+v>`): for selecting blocks of text
- `Command-line`: for running a command `<:>`

---

## Command-line

`:quit` quit (close window)
`:q` quit (close window)
`:w` save (“write”)
`:e {name of file}` open file for editing
`:ls` show open buffers
`:wq` save and quit
`:sp` create new window
`:qa` close all windows
`:help {topic}` open help

- `:help :w` opens help for the :w command
- `:help w` opens help for the w movement
  
## Normal mode

### Basic movement

`k` UP
`j` DOWN
`l` RIGHT
`h` Left

### Words

`w` move cursor one word forward
`b` move cursor one word backward
`e` move cursor end of word

### Lines

`0` move cursor to beginning of line
`$` move cursor to the end of line
`^` move cursor to beginning of empty line

### Screen

`L` move cursor to end of screen
`M` move cursor to middle of screen
`H` move cursor to Higher of screen

### Scroll

`ctrl+u` move cursor to beginning of file
`ctrl+d` move cursor to end of file

### File

`gg` move cursor to beginning of file
`G` move cursor to end of file

### Line numbers

`3w` move 3 words forward
`5j` move 5 lines down
`7dw` delete 7 words

### Find

`f+character` find the next character in the file
`F+character` find the before character in the file
`t+character` find the character but jump 1 character forward before it
`T+character` find the character but jump 1 character backward before it

### Edits

`o` switch from normal mode to insert mode and start a new line below
`O` switch from normal mode to insert mode and start a new line above
`u` undo changes
`d+w` delete the begining a word
`d+e` delete the end of word
`d+$` delete to end of line
`d+0` delete to beginning of line
`c+e` switch to insert mode and delete the end of word
`cw`  change word
`dd` delete the line
`cc` switch to insert mode and delete the line
`x` delete the curent charcter
`r+character` delete the current character and add a new character
`ctrl+r` redo
`yy` copy the current line
`p` paste the current line
`yw` copy the word
`p` past the word

### Modifiers

`ci(` change the contents inside the current pair of parentheses
`ci[` change the contents inside the current pair of square brackets
`da'` delete a single-quoted string, including the surrounding single quotes

---

## Visual Mood

Visual: `v`
Visual Line: `V`
Visual Block: `Ctrl-v`

### Selection

`k` UP
`j` DOWN
`l` RIGHT
`h` Left
`3w` move 3 words forward
`5j` move 5 lines down
`7dw` delete 7 words

### Edits

copy `y`
paste `p`
