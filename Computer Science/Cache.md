# Cache
#cache #memory #register #os 

In order to avoid waiting while we are trying to read/write to RAM, hardware tries to go directly to RAM as rarely as possible. 

What is cache::First time when data is read from RAM, it will then be stored in a place called cache that later can be accessed faster than from RAM.

![[why cache.png]]

---
**Why cache works?**

- The smallest piece of data we can retrieve from memory is a byte. We never cache just a byte. Instead we cache a *cache line* (typically 64 bytes).
- Cache makes programs faster

---

## Write policy

1. **Write-through** - Write to cache line and immediately to memory
2. **Write-back** - Write to cache line and mark cache line as dirty


**Cache coherence protocol** - if there are multiple processor cores

Example: MESI

| Write throught | Write back |
| --- | --- |
| ![[cachethrough.png]]| ![[cacheback.png]] |


**Dirty cache** means that the cache block contains data that is not written for the next datastoring yet.

Write through is simpler and safer, since caching only will contain a copy of data that is found at another place. However if a system wants to provide us with better performace, write-back caching is the way to go.

**Context switch** is when we switch between programs. Cache becomes filled with data from the first program, and it takes time to substitute the data in the cache. So context switch is expensive.


