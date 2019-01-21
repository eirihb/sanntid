# Reasons for concurrency and parallelism


To complete this exercise you will have to use git. Create one or several commits that adds answers to the following questions and push it to your groups repository to complete the task.

When answering the questions, remember to use all the resources at your disposal. Asking the internet isn't a form of "cheating", it's a way of learning.

 ### What is concurrency? What is parallelism? What's the difference?
 > Concurrency: When two or more threads are making progress on a single core switching between them
	Parallelism: When different threads are making progress at same time on different cores.

 ### Why have machines become increasingly multicore in the past decade?
 > Delicline in performance growth for single core
 
 ### What kinds of problems motivates the need for concurrent execution?
 (Or phrased differently: What problems do concurrency help in solving?)
 > Being able to run several programs at the same time
 
 ### Does creating concurrent programs make the programmer's life easier? Harder? Maybe both?
 (Come back to this after you have worked on part 4 of this exercise)
 > probably both, i guess it adds more complex code and possible bugs but allows for efficient solutions for some problems
 
 ### What are the differences between processes, threads, green threads, and coroutines?
 > Process: An executing program than consist of one or several threads. 
Thread: A ordred sequence of instructions that can be processed by a single CPU core
Green threads: scheduled by a library or a VM instead of an OS
Coroutine?
 
 ### Which one of these do `pthread_create()` (C/POSIX), `threading.Thread()` (Python), `go` (Go) create?
 > Create threads
 
 ### How does pythons Global Interpreter Lock (GIL) influence the way a python Thread behaves?
 > It only allows for one thread to execute at a time
 
 ### With this in mind: What is the workaround for the GIL (Hint: it's another module)?
 > Multiprocessing library, each python process gets its own interpreter and memory space
 
 ### What does `func GOMAXPROCS(n int) int` change? 
 > It sets the maximum number of CPUs that can be executing simultaneously

