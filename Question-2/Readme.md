## Question-4.22-Solution

> Note: All the information written below is specific to Ubuntu operating system

### The Code for this Question is - 
[Threaded_Program.c](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-2/Threaded_Program.c)

## Running a Program

The c code file named main.c is kept in the replit(online) repository. Then in shell the code has been compiled and run using commands -

For Compiling -  `gcc -pthread -w main.c`

For Running -  `./a.out`

This program will prompt to ask you to enter the number of elements or values .Then enter all the values on which you want to perform this operation.

After the successful execution of this code we get the required average , minimum and maximum values of the entered values on the screen.

## Screenshot 

![alttext](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-2/Running_a_Program.png)

## Command for getting Time Information

Code - `time ./a.out`

## Screenshot

![alttext](https://github.com/varun-tiwari1/CS252_Assignment/blob/master/Question-2/Time_Information.png)

## Implementation

- The program for calculating the average, minimum and maximum value among given values is written in c programming language.

- Program has three functions named t_avg,t_min and t_max which finds average, minimum and maximum respectively for the input numbers.

- We created 3 threads t1 , t2 and t3 using dataType pthread_t. The above functions are executed in the respective threads created above.

- The average function is operated in thread t1
- The minimum function is operated in thread t2
- The maximum function is operated in thread t3
- Then these threads will execute the respective code for each operation. Then we wait for the thread to terminate using the function pthread_join.If the thread is  already terminated then pthread_join returns immediately.

## pthread Functions used

### pthread_create() function


> int pthread_create(pthread_t *thread, const pthread_attr_t *__restrict__attr, void *(*start_routine)(void *), void *restrict arg);

- First argument is a pointer to pthread_t type that is the data type for threads. It creates a new thread which has already been defined as t1, t2, t3 respectively.

- Second argument is attr pointing to a pthread_attr_t structure to determine attributes for the new thread. In our case attr is given as NULL, as we want the thread to be created with default attributes.

- Third argument is a pointer to the start_routine of a thread. It is the part of the code that is executed by a particular thread.

- Fourth Argument is the argument passed to start_routine(). In our case it is NULL i.e. no arg is passed to our start_routine.

- On success, these functions returns 0

- On error, they return a nonzero error number.

### pthread_join() function

>int pthread_join(pthread_t thread, void **retval);

- The pthread_join() function waits for the thread to terminate. If that thread has already terminated, then pthread_join() returns immediately

- First argument is a pthread_t type that is the data type for threads which has already been defined as t1, t2 and t3 respectively.

- Second argument is retval which specifies the exit status of the thread. If it is not NULL then it has the exit status of thread when pthread_exit() was called. In our case we haven't called pthread_exit() before pthread_join() hence we give argument as NULL.






## References

- C code for calculating average,minimum and maximum - [https://gist.github.com/Jabiribn/e58bf13c678953891900e5f982b48037]() 

- For understanding concept of Threads and Multithreading - CS Minor Lectures by Mr. Mohit P Tahiliani and textbook OS Concepts by Silberchartz

- Websites -

> [https://www.geeksforgeeks.org/thread-functions-in-c-c:~:text=To%20execute%20the%20c%20file,line%20while%20compiling%20the%20file.&text=Syntax%3A,void%20*%2C%20void%20*arg%3B](https://www.geeksforgeeks.org/thread-functions-in-c-c:~:text=To%20execute%20the%20c%20file,line%20while%20compiling%20the%20file.&text=Syntax%3A,void%20*%2C%20void%20*arg%3B)

> [https://www.includehelp.com/c-programming-questions/compiling-program-with-pthread-library-linux.aspx](https://www.includehelp.com/c-programming-questions/compiling-program-with-pthread-library-linux.aspx)

> [https://askubuntu.com/questions/420722/how-to-compile-a-c-program-that-uses-pthread-h](https://askubuntu.com/questions/420722/how-to-compile-a-c-program-that-uses-pthread-h)

> [https://www.ibm.com/docs/en/zos/2.3.0?topic=functions-pthread-create-create-thread#ptcrea](https://www.ibm.com/docs/en/zos/2.3.0?topic=functions-pthread-create-create-thread#ptcrea)



- For understanding Commands and Syntax-
 Websites- [geeksforgeeks](https://www.geeksforgeeks.org/thread-functions-in-c-c/#:~:text=To%20execute%20the%20c%20file,line%20while%20compiling%20the%20file.&text=Syntax%3A,void%20*%2C%20void%20*arg%3B) ,
 [Includehelp](https://www.includehelp.com/c-programming-questions/compiling-program-with-pthread-library-linux.aspx) , [askubuntu](https://askubuntu.com/questions/420722/how-to-compile-a-c-program-that-uses-pthread-h)

- For Assistance Satyam Kalyane- 201IT269 and Lohith N - 201IT133




