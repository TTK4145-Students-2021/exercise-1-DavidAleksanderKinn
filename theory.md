Exercise 1 - Theory questions
-----------------------------
 
 ### What is the difference between concurrency and parallelism?
 > *Bouth in concurrency and in parallelism multiple comutations are done on the same time. The diffrience is that in concurrency the computations don't run simultaneously. Here the diffrient computations done is activly switched. *
 
 ### Why have machines become increasingly multicore in the past decade?
 > *By increasing the number of cores one can run more prosesses in parallel. By running the prosesses in parralell one can increase the preformance speed of programs designed for doing multiple things at the same time. If we have a singel core running at for example 3GHz and, compared to two cores running at 1.5GHz each the multicore vil produce less heat since the power is less. *
 
 ### Why do we divide software (programs) into concurrently executing parts (like threads or processes)?
 (Or phrased differently: What problems do concurrency help in solving?)
 > *If you want the CPU to execute tasks with a starting and finishing time that overlaps, a concurrent program will change the tasks more rapidly. This will make bouth task able to react to input and prosess output at a more steady rate.*
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > * One downside with concurrent programs is that it is more difficult to prevent bugs, esspesualy if two threads writes and read on the same location in memory*
 
 ### What is the conceptual difference between threads and processes?
 > *What is executing the program is one or more treads. The program itself pluss all the threads in it is called a prosess. *
 
 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 > *A green thread is a maintaned by the user not the kernel. This allows green treads to run faster and more (green threads) at the same time. As a downside green threads only suport asynchronous OI, and could be hard to inplement and debug. A coroutine is when multiple functions are executed at the same time (not in parallel), and they are cooperating with each other. For example two funnction changes turns of executing lines of code, and at the same time sends input and resieves output from each other. *
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 > *A gorutine has many of the same characteristics as a thread. Though they are not the same. Gorutine is a rutines which are much smaller than threads. This makes it much cheaper. Gorutines are multiplexed into green treads (green thread stores multiple gorutines). Compared to threads the stack gorutines are stored in are not fixed. This makes it posible to run multiple more gorutiones in one program than threads*
 
 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
 > *This function sets the number of CPUs that can run at the same time. If n is less than 1 then the settings stays the same as before the function was called. *



 
 
 
 
