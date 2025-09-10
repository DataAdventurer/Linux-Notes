A program is an executable file. It contains the code or set of processor instructions that is stored as a file on disk. When the code in a program is loaded into memory and executed by the processor, it becomes a process. An active process also includes the resources the program needs to run. These resources are managed by the operating system. Each process has its own memory address space. One process cannot corrupt the memory space of another process.

A program is an executable file stored on disk. When the code in a program is loaded into memory and executed by the processor, it becomes a process. A process also includes the resources the program needs to run, and these resources are managed by the operating system. Each process has its own memory address space, and one process cannot corrupt the memory space of another process.

The difference between a foreground and background process is that foreground processes are attached to the console. Background processes are not attached.

Every process has a priority, and it is constantly changing, but there is some value called niceness or nice that stays constant unless you change it. Every process on Linux has some kind of nice value, and the nice value is considered when the kernel chooses the priority of each process. Nice basically means how nice the process is to the other processes on your system.

Signals are a way for processes to communicate with one another.


Commands that I learned:
$ ps
$ top
$ jobs
$ bg
$ fg
$ kill
$ killall
$ nice
$ renice
$ nohup
$ halt/poweroff/reboot
$ shutdown


Commands that I used:
$ ps
$ ps x
$ ps aux
$ ps uw 1340
$ top
$ xlogo
$ xlogo &
$ ps
$ jobs
$ fg %1
$ nice -n 10 cpu-hog
$ sudo nice -n -10 must-run-fast 
$ ps
$ renice -n 19 379215
$ xlogo &
$ kill 1738
$ xlogo &
$ kill -1 13546
$ xlogo &
$ kill -INT 13601
$ xlogo &
$ kill -SIGINT 13608
$ kill -l
$ xlogo
$ nohup xlogo
$ xlogo &
$ xlogo &
$ xlogo &
$ killall xlogo



