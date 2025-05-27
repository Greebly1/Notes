
Not all Cache is equal in size and speed. Some caches also perform their own special features.

Note: all types of cache have their own cache controller, and these cache controllers communicate with each other as well as the MMU and the rest of the CPU.
# Diagram
![[CacheHierarchy.png]]

# [[L1 Cache]]
Directly connected to a processor, the smallest and fastest memory besides CPU Registers.

# [[L2 Cache]]
Larger than L1, but smaller and faster than L3. L2 Caches save the processor from doing a slow L3 cache read when an L1 cache miss occurs.

# [[L3 Cache]]
In multicore processors, L3 cache is typically a shared cache between all cores.
Largest and slowest cache, but faster than RAM.

# [[Instruction Cache]]
Modern CPUs support so many specific instructions that it is beneficial to save recently used instructions, especially for algorithmic loops.