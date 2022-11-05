## Question-4.22-Solution

> Note: All the information written below is specific to Ubuntu operating system

### The Code for this Question is - 
[Threaded_Program.c](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-2/Threaded_Program.c)

## Running a Program

The c code file named varun.c is kept in the replit(online) repository. Then in shell the code has been compiled and run using commands -

For Compiling -  `gcc -pthread -w threaded_program.c`

For Running -  `./a.out`

This program will prompt to ask you to enter the number of elements or values .Then enter all the values on which you want to perform this operation.

After the successful execution of this code we get the required average , minimum and maximum values of the entered values on the screen.

## Screenshot 

![alttext](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-2/Running_a_Program.png)

## Implementation

- The program for calculating the average, minimum and maximum value among given values is written in c programming language.

- Program has three functions named t_avg,t_min and t_max which finds average, minimum and maximum respectively for the input numbers.

- We created 3 threads using dataType pthread_t



## References

- C code for calculating average,minimum and maximum - [https://gist.github.com/Jabiribn/e58bf13c678953891900e5f982b48037]() 

- For understanding concept of Threads and Multithreading - CS Minor Lectures by Mr. Mohit P Tahiliani and textbook OS Concepts by Silberchartz

- Websites -

> [https://www.geeksforgeeks.org/thread-functions-in-c-c:~:text=To%20execute%20the%20c%20file,line%20while%20compiling%20the%20file.&text=Syntax%3A,void%20*%2C%20void%20*arg%3B](https://www.geeksforgeeks.org/thread-functions-in-c-c/#:~:text=To%20execute%20the%20c%20file,line%20while%20compiling%20the%20file.&text=Syntax%3A,void%20*%2C%20void%20*arg%3B)

> [https://www.includehelp.com/c-programming-questions/compiling-program-with-pthread-library-linux.aspx](https://www.includehelp.com/c-programming-questions/compiling-program-with-pthread-library-linux.aspx)

> [https://askubuntu.com/questions/420722/how-to-compile-a-c-program-that-uses-pthread-h](https://askubuntu.com/questions/420722/how-to-compile-a-c-program-that-uses-pthread-h)

> [https://www.ibm.com/docs/en/zos/2.3.0?topic=functions-pthread-create-create-thread#ptcrea](https://www.ibm.com/docs/en/zos/2.3.0?topic=functions-pthread-create-create-thread#ptcrea)



- For understanding Commands and Syntax-
 Websites- [geeksforgeeks](https://www.geeksforgeeks.org/thread-functions-in-c-c/#:~:text=To%20execute%20the%20c%20file,line%20while%20compiling%20the%20file.&text=Syntax%3A,void%20*%2C%20void%20*arg%3B) ,
 [Includehelp](https://www.includehelp.com/c-programming-questions/compiling-program-with-pthread-library-linux.aspx) , [askubuntu](https://askubuntu.com/questions/420722/how-to-compile-a-c-program-that-uses-pthread-h)

- For Assistance Satyam Kalyane- 201IT269 and Lohith N - 201IT133




