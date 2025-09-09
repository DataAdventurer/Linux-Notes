Every file and directory in your Linux system will have three permissions groups. There is owner, which is permissions for who owns this file or directory. Group permissions apply to the group assigned to the file or directory. Others permissions are what all the other users have, and you have to be diligent to protect them. Each permission group gets three permissions: read, write, and execute. Linux scoring system: read gets 4, write gets 2, and execute gets 1. 775 would give owner rwx, group rwx, and others rx.

Umask controls the permissions with which a user can create new files and directories. Umask works by doing a bitwise AND with the bitwise complement.

Setgid
If the file is an executable file, when you execute it, it will take on the group owner’s permissions. For a directory, any new files or directories placed in this directory will inherit the group owner.

Sudo is an acronym for super user do. It is a command that runs with elevated permissions without the need to change your identity.

Su, on the other hand, is an acronym for switch user. You are basically switching to a particular user, and you need the credentials for the user you are switching to.


Commands that I learned:
$ id
$ chmod
$ umask
$ su
$ sudo
$ chown
$ chgrp
$ addgroup
$ usermod
$ passwd


Commands that I used:
$ file /etc/shadow
$ less /etc/shadow
$ id
$ > foo.txt
$ ls -l foo.txt
$ chmod 600 foo.txt
$ ls -l foo.txt
$ rm -f foo.txt
$ umask
$ > foo.txt
$ ls -l foo.txt
$ rm foo.txt
$ umask 0000
$ > foo.txt
$ ls -l foo.txt
$ sudo -l
$ sudo groupadd music
$ sudo usermod -a -G music janet
$ sudo usermod -a -G music tony

