https://en.wikipedia.org/wiki/MESI_protocol
An **Invalidation-based [[Cache Coherence]] Policy**
	It provides a system to check whether a cache-line is valid

Also known as the **Illinois Protocol**

MESI is a newer advanced form of an older but similar [[MSI]] Cache Coherence policy.
# States
The 4 letters of MESI represent the 4 states a cache-line can be in.
	A cache line actually has 2 states of these 4 states at any given time, represented by a pair of 2 bits.

**M - Modified**
	The cache-line is only present in this cache and has been modified, it is *dirty*. It must be written back to memory at some point. When the write-back occurs it switches to the S-Shared state.
**E - Exclusive**
	The cache line is present only in the current cache, but is _clean_ - it matches main memory. It may be changed to the Shared state at any time, in response to a read request. Alternatively, it may be changed to the Modified state when writing to it.
**S - Shared**
	Indicates that this cache line may be stored in other caches of the machine and is _clean_ - it matches the main memory. The line may be discarded (changed to the Invalid state) at any time.
**I - Invalid**
	This cache-line is invalid, perhaps it has been modified by another high level cache, and it is awaiting its write-back. 

#TODO 
More on the state machine aspect of MESI