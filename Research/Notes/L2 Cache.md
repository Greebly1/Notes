
When an [[L1 Cache]] miss occurs, accessing [[L3 Cache]] is slow at this timescale.

L2 cache is larger and slower than L1, however it is much smaller than L3, thus it is much faster.
	L2 caches save the processor from slow L3 cache reads after an L1 cache miss

# Size
~256KB-2MB per core

# Private
In most systems L2 cache is private to the core it is attached to. It also has its own individual cache controller.

# Exclusivity
L2 cache typically is 'exclusive' to L1, meaning it will never store duplicate data, meaning it save precious space. 

# Data Pre-Fetch Speculating
Cutting edge [[CPU Speculation]] systems look forward in the instructions to see future memory address reads. Then prefetch the data into the L2 cache.