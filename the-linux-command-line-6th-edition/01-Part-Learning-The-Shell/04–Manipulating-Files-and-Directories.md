Most frequently used Linux commands are cp, mv, mkdir, rm and ln. 

Wildcard:            Meaning:
*                    Matches any character
?                    Matches any single character


Example:
*   , all fiels
*g  , Any file beginning with “g”
b*  , Any file beginning with “b” followed by any characters and ending with “.txt”







Commands that I learned:
$ cd
$ mkdir playground
$ cd playground
$ mkdir dir1 dir2
$ cp /etc/passwd .
$ mv passwd fun
$ mv fun dir1
$ ls -l dir2/dir1

Hard links:
"A hard link is the file-system representation of a file by which more than one path references a single file in the same volume."
$ ln fun fun-hard
$ ln fun dir1/fun-hard
$ ln fun dir2/fun-hard

Symbolic Links:
"Symbolic links are a special type of file that contains a text pointer to the target file or directory."
$ ln -s fun fun-sym
$ ln -s ../fun dir1/fun-sym
$ ln -s ../fun dir2/fun-sym
$
$

