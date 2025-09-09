Script
It records a shell session for you so that you can look at the output you saw at the time, and you can even record with timing.


Commands that I learned:
$ clear
$ history

Cursor Movement:
Ctrl-a    Move cursor to the beginning of the line.
Ctrl-e    Move cursor to the end of the line.
Ctrl-f    Move cursor forward one character; same as the right arrow key.
Ctrl-b    Move cursor backward one character; same as the left arrow key.
Alt-f     Move cursor forward one word.
Alt-b     Move cursor backward one word.
Ctrl-l    Clear the screen and move the cursor to the top-left corner. The clear command does the same thing.

Ctrl-d    Delete the character at the cursor location.
Ctrl-t    Transpose (exchange) the character at the cursor location with the one preceding it.
Alt-t     Transpose the word at the cursor location with the one preceding it.
Alt-l     Convert the characters from the cursor location to the end of the word to lowercase.
Alt-u     Convert the characters from the cursor location to the end of the word to uppercase.

Ctrl-k    Kill text from the cursor location to the end of line.
Ctrl-u    Kill text from the cursor location to the beginning of the line.
Alt-d     Kill text from the cursor location to the end of the current word.
Ctrl-y    Yank text from the kill-ring and insert it at the cursor location.

History Commands:
Ctrl-p    Move to the previous history entry. This is the same action as the up
arrow.
Ctrl-n    Move to the next history entry. This is the same action as the down
arrow
Alt-<     Move to the beginning (top) of the history list.
Alt->     Move to the end (bottom) of the history list, i.e., the current command line.
Ctrl-r    Reverse incremental search. This searches incrementally from the current command line up the history list.
Alt-p     Reverse search, nonincremental. With this key, type in the search string and press enter before the search is performed.
Alt-n     Forward search, nonincremental.
Ctrl-o    Execute the current item in the history list and advance to the next one. This is handy if we are trying to re-execute a sequence of commands in the history list.



Commands that I used:
$ history | less
$ history | grep /usr/bin
$ !245
$ !ls:p

