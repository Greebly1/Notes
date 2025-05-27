

Memory ranged may be flagged as non-cacheable to the [[Memory Controller]] for a number of reasons.

For example, a real time clock module may have a read only register that gives a 64 bit real world clock time. Any cache value of this register would be invalid since the time moves forward constantly.

Non-Cacheable Memory addresses must always be done with a full memory read
	Better data reliability
	Better precision

# [[MMIO]]
Typically Memory mapped I/O is not cacheable, since external devices may write to those locations, invalidating any cache that exists in the CPU.

Some memory controllers however can listen for MMIO calls on the address bus and invalidate their own cache.

A simpler solution though is to just mark any MMIO region as non-cacheable

