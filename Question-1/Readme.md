## Question- 2.24 Solution

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

## Implementation

- The program of copying the contents from source file and pasting it to destination file is written in c programming language.

- The input file was copy.txt from where we copied the contents.

- The output file was paste.txt to which we copied the contents.

- The commands discussed above to compile and run the code in order to perform the copy paste operation.

- Then strace log file is created to keep track of all the system calls made during this operation. 

## References

- C code for copy-paste operation - geeksforgeeks

- For understanding system calls- websites like gfg,stackoverflow.OS Concepts mentioned above,You Tube.

- For understanding commands and syntax- websites like gfg,stackoverflow,man7.org,etc

- For assistance Dev Agrawal-
201ME169 and Vincent Paul- 201ME365
