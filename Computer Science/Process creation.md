# Process creation

**Topic**: #os
**Relevant topics**:  #process 
**Info sources**: 
**Additional tags**: #flashcardsos #review
**Description**: 


## How does process creation work?

1. To run a program, OS loads its code and any static data into memory. Into the adress space of the process.
2. Programs initially reside on disk in some kind of executable format. Thus, the process of loading a program and static data into memory requires the OS to read from bytes from disk and place them in memory somehow.
3. Before it happened eagerly. Nowadays it happens lazily.
4. Some memory must be allocated for the program's run-time stack ([[Run-time stack|stack]])
5. OS will likely initialize the stack with arguments: argc and argv array
6. OS may also create some initial memory for the program's [[Heap|heap]]
7. Start the program running at the entry point, namely <code>main()</code>
8. The OS transfers control of the CPU to the newly-created process.
9. Program begins execution.


## Questions

- Question one: Answer (Add colon)
- Question two: Answer


## Other notes

- first
