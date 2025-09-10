Environment variables set a number of variables for your shell environment. Environment variables are important because applications, command-line tools, and shell scripts use them to determine their configuration.

Linux systems provide a shortcut system with the dollar sign and the PATH variable. For example, /usr/local/sbin: contains directories separated by colons. Linux will go through each directory in order when you type the name of a command like ls. When you type ls, the operating system checks the first directory in PATH for an executable named ls. If it is not there, it checks the next, and so on.

In an operating system, a process has to be instantiated, meaning created by another process. The process which creates another process is called the parent process. The created process is called the child process.

.bashrc is called every time a new shell is started in interactive mode. Whenever a new shell is opened, this file will run. .bash_profile is called only the first time when you log into the shell. .bash_logout is called whenever you log out from the shell. On login, .bash_profile runs first. .bashrc is often run from within .bash_profile. In practice, .bashrc runs for interactive shells, while .bash_profile runs for login shells. That is why sometimes it looks like .bashrc runs first, depending on how the files are configured.

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
