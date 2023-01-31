**Definition:** Synchronization refers to the coordination of events between different threads wrt time

Threads run in random orders and can cause conflicts, need synchronization (most of the time) to get consistent results

`join()` method - Program stops executing until the thread it’s called on is terminated
	– Throws InterruptedException if interrupted
	– Don’t start then join then start then join, basically makes the program not multi-threaded

### Concurrent Program Errors:
Race Condition - When the order of operations are performed affect their correctness

Data Race - Concurrent access by different threads to the same variable, where at least one writes to it

### Locks
**Definition:** An entity that can only be held by one thread at a time
- Threads acquire locks and release them when done with the object
- If one thread has a lock all other threads that need the object go into a blocked state
Ex:
```
static Object o = new Object();
synchronized(o) {
...
}
```
	- Thread releases lock when it leaves sychronized block for any reason

Synchronized keyword can also be applied to methods, which obtain a lock for execution of whole body

