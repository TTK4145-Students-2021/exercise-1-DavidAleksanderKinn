Exercise 1 - Theory questions
-----------------------------
 
 ### What is the difference between concurrency and parallelism?
 > Both in concurrency and in parallelism multiple comutations are done on the same time. The diffrience is that in concurrency the computations don't run simultaneously. Here the diffrient computations done is activly switched. 
 
 ### Why have machines become increasingly multicore in the past decade?
 > By increasing the number of cores one can run more processes in parallel. By running the processes in parallel one can increase the performance speed of programs designed for doing multiple things at the same time. If we have a singel core running at for example 3GHz and, compared to two cores running at 1.5GHz each the multicore vil produce less heat since the power is less. The clocktime on CPU's becomes harder and harder to increase, and by having CPU's in parallel we can increase the overall speed, without increasing clocktime.
 
 ### Why do we divide software (programs) into concurrently executing parts (like threads or processes)?
 (Or phrased differently: What problems do concurrency help in solving?)
 > If you want the CPU to execute tasks with a starting and finishing time that overlaps (natural parallelism), a concurrent program will change the tasks more rapidly. This will make both task able to react to input and process output at a steadier rate.
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > Concurrent programs make it easier to program processes which intentionally should run in parallel. One downside with concurrent programs is that it is more difficult to prevent bugs, especially if two threads write and read on the same location in memory
 
 ### What is the conceptual difference between threads and processes?
 > What is executing the program is one or more treads. The program itself pluss all the threads in it is called a process. Processes do not share memory, but threads do. 
 
 ### Some languages support "fibers" (sometimes called "green threads") or "coroutines"? What are they?
 > A green thread is a maintained by the user not the kernel. This allows green treads to run faster and for a prosses to contain more threads (more light weighted). As a downside, green threads only support asynchronous OI and could be hard to implement and debug. A coroutine is when multiple routines are executed at the same time (with concurrency, not in parallel), and they are cooperating with each other. They very light weighted. For example, two function changes turn of executing lines of code, and at the same time sends output and receives input of when one is finished execution and when one should start. This way of concurrency could provide control over what's running when, but could also be risky since it is depending on the routines communicating. 
 
 ### What is the Go-language's "goroutine"? A C/POSIX "pthread"?
 > Goroutines is Go's implementation of a coroutine. This implementation is made very userfriendly, which is one of many good quality with Go.
 
 ### In Go, what does `func GOMAXPROCS(n int) int` change? 
 > This function lets the program know how many threads that are distrbuted to it, and can use this information to know how many goroutines the program could execute. 


 
 
 
 
