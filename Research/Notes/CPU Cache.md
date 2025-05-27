

A fast temporary data storage for the CPU.
If a register is the CPUs hands, then the cache is the CPU's pockets.

Caches store frequently used data, and data that is expected to be used soon. 

Caching systems are done automatically, not handled by the ISA but improve access speeds at a hardware level by 'already having the data ready before it is read'

# Note on Hard Drive Memory
CPU cache typically only handles main memory, AKA RAM.
	In some specific setups hard drive memory may be cached, however typically hard drive cache systems operate at a software level handled by the OS.
Some hard drive modules contain small caches for reading and writing fast, but those differ by manufacturer

# Cache Lines
Cache works fast by essentially being a giant block of ram inside the CPU, that get swapped out with chunks of RAM expected to be accessed next. 
	These chunks are called #Cache-Lines

A Cache line is typically 64 bytes long.

# Translation Lookaside Buffer [[TLB]]
When the CPU reads from RAM, the Cache controller first checks its Translation Lookaside Buffer TLB, to see if that value already exists in cache.

Likewise when data is added or removed to the cache, the TLB is updated to match

# [[Replacement Policy]]
Different cache systems utilize different replacement policies for when to overwrite old cache with new data.

# [[Write Policy]]
Cache systems may also handle writes differently. With 2 main ways of handling writes.

# [[Cache Coherence]]
Various circumstances can cause cache to no longer be valid
A cache system must be able to ensure data in cache is valid, they will implement a type of Cache Coherence Policy.

# [[Cache Hierarchy]]
In modern multicore processors, there are multiple levels of CPU cache with varying speeds.
L1
L2
L3