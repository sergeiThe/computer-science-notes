# Threads, symmetric multiprocessing (SMP) & microcore
#threads #smp #core 

## Process from an OS worldview

1. Process'es access to resources
2. Planning, execution


**[[Thread]]** - element of process execution
**[[Task]]** - element of ownership (how much memory f.ex)

## Thread

Process inside a process

[[Multithreading]]

![[threads1.png]]

Box - process
Dotline - thread

Threads in a process:
- State
- Context
- Stack of execution
- Local data
- Access to processor resources

Thread is a child of a process.
Threads use one address space.
Switching between threads is faster that switching between processes.

![[threads2.png]]

## Why?

- Speed
- Communication between threads does not involve the kernel


Pause of a process, pauses also the threads inside the process.

Threads are not parallell. They switch like processes. Just faster.

## Kernel-level threads

![[kernelthreads.png]]

**Pros**
- OS knows about the threads and can manage them and their processes
- Suits will for applications with frequent blocking
- Internal operations of the OS can use multithreading

**Cons**
- Management switch between threads happens through the kernel
- Slow
- Extra cost for managing


## User-level threads

![[uselevelthreads.png]]

**Pros**
- For OS that does not support multithreading 
- Incorporation of user threads does not require OS modifications 
- Threads are presented simply
- Working with threads is simple, does not include interaction with the kernel
- High speed of switching between threads

**Cons** 
- OS does not know about threads, so it can potentially poorly manage processes.

(Solaris)

## Symmetric multiprocessing

Traditional approach:
- Processor executes one instruction at a time
- Each instruction is a pipeline of operations

[[Symmetric multiprocessing]]

[[Clusters]] 

[[SISD]]

[[SIMD]]

[[MIMD]]

