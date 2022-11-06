## Question- 2.24 - Solution

> Note: All the information written below is specific to Ubuntu operating system

## Running the program

- The c code file named varun.c is kept in the replit(online) repository. Then in shell the code has been compiled and run using commands -

For compiling- `gcc -w varun.c`

For running- `./a.out`

- This program will prompt to ask you to enter the source file and the destination file.

- After the successful execution of this code the Success message will prompt to your screen.

## Screenshot

![alt text](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-1/run_code_shell_image.png)

## Command to create an log file to track all the system calls in this operation

- Command- `strace -ostrace_log ./a.out`

- The command will prompt the user to provide the name of the source file and the destination file

- If it has been executed successfully, a "Success" message will be prompted to the screen(shell).

## Screenshot

![alt text](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-1/strace_log_Execution.png)

## System Calls log file

[strace_log file](https://github.com/varun-tiwari1/CS252_Assignment/commit/8ac0816d127468581176d3f91b17075c09f82188)

## Number of times Each Systems Call is Called

Command - `strace -c ./a.out`

## Screenshot

Table of System Calls

![alttext](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-1/System_calls_table.png)

## Implementation

- The program of copying the contents from source file and pasting it to destination file is written in c programming language.

- The input file was copy.txt from where we copied the contents.

- The output file was paste.txt to which we copied the contents.

- The commands discussed above to compile and run the code in order to perform the copy paste operation.

- Then strace log file is created to keep track of all the system calls made during this operation. 

## List of Some System Calls in this operation

### 1. openat
- Open a file relative to a directory file descriptor

### 2. read
- Reads from a file descriptor

### 3. write
- Writes to a file descriptor

### 4. close 
- Closes a file descriptor

### 5. mmap
- map files or devices into memory

### 6. brk
- change data segment size

### 7. access
- checks whether the calling process can access the file pathname.

### 8. pread64
- read from a file descriptor at a given offset

### 9. mprotect
- set protection on a region of memory

### 10. lseek
- reposition read/write file offset


## References

- C code for copy-paste operation -
> https://www.geeksforgeeks.org/c-program-copy-contents-one-file-another-file/

- For understanding system calls- websites like gfg,stackoverflow.OS Concepts mentioned above,You Tube.

-Websites

> https://www.geeksforgeeks.org/introduction-of-system-call/

>https://www.guru99.com/system-call-operating-system.html


- For understanding Commands and Syntax- websites like 
> https://www.geeksforgeeks.org/strace-command-in-linux-with-examples/

- For Assistance of code Dev Agrawal-
201ME169 and Vincent Paul- 201ME365
