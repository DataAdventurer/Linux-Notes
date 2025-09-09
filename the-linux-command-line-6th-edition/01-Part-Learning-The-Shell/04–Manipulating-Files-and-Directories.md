Wildcards are symbols or sets of symbols that represent other characters in a search or pattern matching operation. They are commonly used in file searches, programming, and database queries to simplify criteria.

Any filename that starts with a dot is considered a hidden file. Files are hidden to prevent users from accidentally modifying or deleting important system files.

Most frequently used Linux commands are cp, mv, mkdir, rm and ln. 

Wildcard:            Meaning:
*                    Matches any character
?                    Matches any single character


Example:
*   , all fiels
*g  , Any file beginning with “g”
b*  , Any file beginning with “b” followed by any characters and ending with “.txt”

Commands that I used on lesson:
$ cd
$ mkdir playground
$ cd playground
$ mkdir dir1 dir2
$ cp /etc/passwd .
$ ls -l
$ cp -v /etc/passwd .
$ cp -i /etc/passwd .
$ mv passwd fun
$ mv fun dir1
$ mv dir1/fun dir2
$ mv dir2/fun .
$ mv fun dir1
$ mv dir1 dir2
$ ls -l dir2
$ ls -l dir2/dir1
$ mv dir2/dir1 .
$ mv dir1/fun .


Hard links:
"A hard link is the file-system representation of a file by which more than one path references a single file in the same volume."
$ ln fun fun-hard
$ ln fun dir1/fun-hard
$ ln fun dir2/fun-hard
$ ls -l
$ ls -li

Symbolic Links:
"Symbolic links are a special type of file that contains a text pointer to the target file or directory."
$ ln -s fun fun-sym
$ ln -s ../fun dir1/fun-sym
$ ln -s ../fun dir2/fun-sym
$ ls -l dir1
$ ln -s /home/me/playground/fun dir1/fun-sym
$ ln -s dir1 dir1-sym
$ ls -l
https://www.youtube.com/watch?v=lW_V8oFxQgA