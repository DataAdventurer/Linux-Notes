Shell expansion
The command is given, the first thing that's going to happen is the interpreter is going to break this into tokens. Each token is expanded, then quotes are removed. The command is then interpreted. When an unquoted token is expanded in the shell, special pattern matching characters cause Bash to search the filesystem for matches.

Brace expansion
"Brace expansion is useful because it provides a concise, efficient way to generate lists of strings (like filenames or command-line arguments) from a single pattern, saving typing and reducing complexity in commands and scripts."

Arithmetic expansion
Arithmetic expansion is a shell feature that allows users to do simple integer based arithmetic operations.


Commands that I learned:
$ echo

Commands that I used:
$ echo this is a test
$ echo *
$ ls
$ echo D*
$ echo *s
$ echo ~
$ echo ~bob
$ echo $((2 + 2))
$ echo $(((5**2) * 3))
$ echo Front-{A,B,C}-Back
$ echo Number_{1..5}
$ echo {01..15}
$ echo {001..15}
$ echo {Z..A}
$ echo a{A{1,2},B{3,4}}b
$ mkdir Photos
$ cd Photos
$ mkdir {2007..2009}-{01..12}
$ ls
$ echo $USER
$ printenv | less
$ echo $(ls)
$ ls -l $(which cp)
$ file $(ls -d /usr/bin/* | grep zip)
$ ls -l `which cp`
$ echo this is a test
$ echo The total is $100.00
$ ls -l two words.txt
$ ls -l two words.txt
$ ls -l "two words.txt"
$ mv "two words.txt" two_words.txt
$ echo "$USER $((2+2)) $(df -h)"
$ echo $(df -h)
$ echo "$(df -h)"
$ echo "The balance for user $USER is: \$5.00"
$ mv bad\&filename good_filename
