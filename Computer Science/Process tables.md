# Process table
#process #batch #fork #pt #os

The process table (PT) contains an entry for each [[Processes|process]] present in the system. 

The entry is created when the process is created by a Fork system call. 

Each entry contains several fields that stores all the information pertaining to a single process.

The maximum number of entries in PT (which is maximum number of processes allowed to exist at a single point of time in eXpOS) is MAX_PROC_NUM. In the current version of eXpOS, MAX_PROC_NUM = 16.