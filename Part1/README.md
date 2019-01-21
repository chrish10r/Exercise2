# Mutex and Channel basics

### What is an atomic operation?
> *An operation during which a processor can simultaneously read a location and write it in the same bus operation. This prevents any other processor or I/O device from writing or reading memory until the operation is complete. 

Atomic implies indivisibility and irreducibility, so an atomic operation must be performed entirely or not performed at all.*

### What is a semaphore?
> *A semaphore is a synchronization object that controls access by multiple processes to a common resource in a parallel programming environment. Semaphores are widely used to control access to files and shared memory. The three basic functionalities associated with semaphores are set, check and wait until it clears to set it again.*

### What is a mutex?
> *Mutex is a program object that allows multiple program threads to share the same resource, such as file access, but not simultaneously.*

### What is the difference between a mutex and a binary semaphore?
> *Both do the same thing: locking a resource. The semaphore is like a post-it note. It declare wether the resource is in use, but anyone can in principle change it. Mutex is more like a key; it locks the door, preventing anyone but itself from using it.*

### What is a critical section?
> *The critical section is the part of the code that's being controlled/locked by a semaphore/mutex.*

### What is the difference between race conditions and data races?
 > *A race condition can occur when timing or ordering is essential. When the order is broken becouse of parallell operations, we call it a race condition. Data races happenswhen two processors access the same memory location at the same time. Since both can read and write to it, there are no way of knowing whats on the location.*

### List some advantages of using message passing over lock-based synchronization primitives.
> *Message passing doesn't have global variables and it's "easier" to implement.*

### List some advantages of using lock-based synchronization primitives over message passing.
> *It is a lot faster as you are working directly with the memory. Message passing has a limit of how much data can be sent.*
