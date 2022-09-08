# Operating systems
#os #virtualization #resources #cpu #memory 

Operating systems [[Virtualization|virtualize]] physical resources so they become user friendly and manage resources of a computer. 

## Main tasks

- Virtualizing CPU 
- Virtualizing memory
- [[Concurrency]]
- [[Persistence]]


## OS design goals

1. Virtualization - create abstractions
2. Performance - minimize overhead
3. Security - protect/isolate applications
4. Reliability - stability
5. Energy-efficient - environmentally friendly


## [[Processes]]

- Policy vs mechanism
- Process vs program
- Creation
- States
- Process list

**Batch processing** is the processing of previously collected jobs in a single batch.


### Process characteristics

CPU-bound - scientific computing, machine learning, multimedia
*Hyperthreading does not help cpu-bound processes*

I/O-bound - not much to do, mostly wait for I/O

Memory-bound - heavy use of memory (often also cpu-bound)

Real-time - have deadlines, soft real-time (multimedia) vs hard-time (robotics)

Batch vs interactive - batch has no I/O

Service - the ones that run without any user logged in as opposed to a user processs

