Everything on a computer is just a stream of bytes. This idea reflects the fact that any user action results in reading or writing bits at addresses controlled by the operating system. We can also say that “everything appears somewhere in the file system.”

Soft Link:
Soft link is like a shortcut in Windows. It is a pointer. File pointing to another file. The file size of a soft link is usually smaller than the size of the original file. The inode number of a soft link is different from the inode number of the original file.

Hard Link:
Hard link is another name for the same file. It has the same file size and the same inode number. If the original file is deleted, the hard link is not affected. It is like a duplicate entry for the same file.

"Plain text files are the simplest form of configuration files and are easy to read and write. They are often used in Unix-like operating systems, where they configure the system and applications."


The /bin directory stands for binary and includes the binaries or executables required for the system to function. Modern Linux systems put these in /usr/bin. /sbin is similar to the /bin directory but contains applications only the superuser would need. /usr, nowadays, can contain a long list of things that need to be shared by apps and services. The /opt directory stands for optional and is where software that you build and compile is placed. /etc is an important folder where you will find system-wide configuration files. /home is the personal directory. The /boot directory contains the files needed to boot a Linux computer. The /lib folder is where libraries are kept for system programs. The /root folder is the home directory of the superuser. The /tmp directory contains temporary files placed there by apps that are running. The /var directory contains logs and also temporary files used between reboots. The /dev folder is where device files are kept.


ls command possible options.
$ ls -a
List all files also the hidden ones.
$ la -A
Does almost same job than -a but not included current directory and parent directory.
$ ls -S
Sort results by file size.
$ ls -l
Display results in long format.

You can see some file rights and it looks like this:
-rw-r--r-- 
Owner can read and write. Group can only read. Others can also only read.
You can also see who created the file and the name of the group who owns the file. Other things you can see about the file are the date and time it was modified, and the size of the file in bytes.

Commands that I learned:
$ ls /usr
$ ls ~ /usr
$ ls -l
$ ls -lt --reverse
$ less /etc/passwd
$ cd /proc           and many others
