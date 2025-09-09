The four commands in Linux are an executable program, a command built into the shell itself shell function and an alias.

Type: is a shell builtin that displays the kind of command the shell will execute given particular command name.

man PAGE
Man is short for manual. A man page is documentation. Man is the built-in help system in Linux. Only one hyphen (dash) is needed for multiple single-character options.

The alias command is used for creating command shortcuts and abbreviations, which can significantly enhance your productivity and customize your Linux experience. It also reduces typing errors.


Commands that I learned:
$ type
$ which
$ help
$ man
$ apropos
$ info
$ whatis
$ alias

Commands that I used:
$ type type
$ type ls
$ type cp
--
$ which ls
$ which cd
--
$ help cd
$ mkdir --help
--
$ man 5 passwd

Creating Own Commands with alias
$ cd /usr; ls; cd -
$ type test
$ type foo
$ alias foo='cd /usr; ls; cd -'
$ foo
$ type foo
$ unalias foo
$ type foo
$ type ls
$ alias