Threads can be executed in parallel by hardware

**Process Definition:** A program loaded into memory and executing

**Thread Definition:** a sequentially executed sequence of instructions inside a process
	– Threads share the same data with other threads in their process
	– Each thread has its own local variables

Two approaches to creating threads:
1. Extend the thread class
	`public class ThreadHelper extends Thread`
	`ThreadHelper mt = new ThreadHelper();`
2. Implement the Runnable Interface (better way)
	`public class ThreadHelper implemenets Runnable`
	`Thread t = new Thread(new ThreadHelper()) `

After thread is instantiated:
- Put the processes to be performed in the run() method
- Call `start()` on each of the thread objects

Thread States:
- New → Allocated and waiting for `start()`
- Waiting → It can begin execution
- Runnable → Currently executing
- Blocked → Waiting for event
- Terminated → Finished

The order that threads are run is indeterminate