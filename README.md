# Operating-System

Q.N.1 
In this question we need to create a process that in turn creates a child process and that child process will output some sequence. For ex. if 8 is passed as a parameter on the command line, the child process will output 8, 4, 2, 1. In the concept of operating system the system call used for creating the child process is Fork(). This system call creates a child process and returns an integer value. Depending on that integer value we get the idea whether the child process is created or not. If the process returns the value -1 indicates that the child process has not been created. If the value returned is 0 then it indicates that the child process is created.
We need to prevent the parent process from completing before the child process because the child process will become orphan process. Therefore to prevent this we need to use the system call wait() so that the child process completes before the parent process.

Q.N.2
In this question we have to make a program named which implements the concept of file. The programs demands to be passed two parameters the name of the file having the content and the name of the file in which the content needs to be copied. The concept behind using pipe is to perform the interprocess communication such that one process writes to the pipe and the other process reads from that pipe. Pipe is a one way communication process.
The program asks to perform communication in such a way that the parent process writes into the pipe and then the child process will read from the pipe and copy it into the destination file using pipe.
