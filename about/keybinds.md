---
layout: default
title: Keybinds
parent: About
permalink: /about/keybinds
---

## Keybinds
These are the available keybinds which termcrypt can use while in input mode.

### Emacs mode (default mode)

Keystroke    | Action
---------    | ------
Ctrl-A, Home | Move cursor to the beginning of line
Ctrl-B, Left | Move cursor one character left
Ctrl-E, End  | Move cursor to end of line
Ctrl-F, Right| Move cursor one character right
Ctrl-H, Backspace | Delete character before cursor
Ctrl-I, Tab  | Next completion
Ctrl-K       | Delete from cursor to end of line
Ctrl-L       | Clear screen
Ctrl-N, Down | Next match from history
Ctrl-P, Up   | Previous match from history
Ctrl-X Ctrl-U | Undo
Ctrl-Y       | Paste from Yank buffer (Meta-Y to paste next yank instead)
Meta-<       | Move to first entry in history
Meta->       | Move to last entry in history
Meta-B, Alt-Left | Move cursor to previous word
Meta-C       | Capitalize the current word
Meta-D       | Delete forwards one word
Meta-F, Alt-Right | Move cursor to next word
Meta-L       | Lower-case the next word
Meta-T       | Transpose words
Meta-U       | Upper-case the next word
Meta-Y       | See Ctrl-Y
Meta-Backspace | Kill from the start of the current word, or, if between words, to the start of the previous word
Meta-0, 1, ..., - | Specify the digit to the argument. `–` starts a negative argument.

[Readline Emacs Editing Mode Cheat Sheet](http://www.catonmat.net/download/readline-emacs-editing-mode-cheat-sheet.pdf)