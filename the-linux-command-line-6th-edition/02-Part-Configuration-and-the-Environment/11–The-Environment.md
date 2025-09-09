
Stored enviroment is when shell stores two basic types of data in the enviroment tough. They are environment variables and shell variables.




Commands that I learned:
$ printenv
$ set
$ pexports
$ alias
$ source




Commands that I used:
$ printenv | less
$ printenv USER
$ set | less
$ echo $HOME
$ alias
$ foo="bar"
$ bash
$ ps
$ echo $foo
$ exit
$ ps
$ echo $foo
$ MANWIDTH=75 man ls
$ alias man=’MANWIDTH=75 man’
$ cp .bashrc .bashrc.bak
$ nano .bashrc
    # Change umask to make directory sharing easier
    umask 0002
    # Ignore duplicates in command history and increase
    # history size to 1000 lines
    export HISTCONTROL=ignoredups
    export HISTSIZE=1000
    # Add some helpful aliases
    alias l.='ls -d .* --color=auto'
    alias ll='ls -l --color=auto'
$ source ~/.bashrc
$ ll
