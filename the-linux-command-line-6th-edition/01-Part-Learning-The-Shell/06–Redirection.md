Standard input is where programs normally get their input, which is the keyboard most of the time, but in Linux this can actually be redirected to come from another device or a file. Standard input is referred to as file descriptor 0.

Standard output is the default output device for programs, normally your terminal or screen. Standard output is referred to as descriptor 1.

Standard error is also normally your terminal but is especially made for error messages. Standard error is referred to as file descriptor 2. These numbers 0, 1, and 2 will be used later on when we use redirections in the shell. Both standard output and standard error can be redirected just like standard input.

A pipe (|) is used to send the output to another command, whereas redirection (>) is used to redirect the output to a file.

/dev/null is a virtual device. Any data written to /dev/null vanishes or disappears. It is also called the bit bucket or black hole.

"The central idea of the Unix Philosophy is to build composable components that do one thing well. Small minimalist components are easier to understand and modify which allows for faster experimentation. New features are added by connecting to existing components or creating a new component. Higher order functionality then emerges from the connections between components."


Commands that I learned:
$ cat
$ sort
$ uniq
$ grep
$ wc
$ head
$ tail
$ tee

Commands that I used:
$ ls -l /usr/bin > ls-output.txt
$ ls -l ls-output.txt
$ less ls-output.txt
$ ls -l /bin/usr > ls-output.txt
$ ls -l ls-output.txt
$ > ls-output.txt
$ ls -l /usr/bin >> ls-output.txt
$ ... .x 3
$ ls -l ls-output.txt
$ ls -l /bin/usr 2> ls-error.txt
$ ls -l /bin/usr > ls-output.txt 2>&1
$ ls -l /bin/usr 2> /dev/null
$ cat ls-output.txt
$ cat > lazy_dog.txt
$ cat lazy_dog.txt
$ cat < lazy_dog.txt
$ ls -l /usr/bin | less
$ ls /bin /usr/bin | sort | less
$ ls /bin /usr/bin | sort | uniq | less
$ ls /bin /usr/bin | sort | uniq -d | less
$ wc ls-output.txt
$ ls /bin /usr/bin | sort | uniq | wc -l
$ ls /bin /usr/bin | sort | uniq | grep zip
$ head -n 5 ls-output.txt
$ tail -n 5 ls-output.txt
$ ls /usr/bin | tail -n 5
$ tail -f /var/log/messages
$ ls /usr/bin | tee ls.txt | grep zip
