
The largest and slowest cache, still faster than main memory/RAM

# Size
~4MB-64MB

# Shared
L3 is a special shared cache, meaning that all CPU cores can access the L3 cache. While this does make it the slowest cache, inclusivity essentially allows cores to share L1 and L2 caches indirectly.

# Inclusivity
The L3 Cache will 'mirror' the data that is inside L2 and L1. Effectively this allows all cores to share their cache through the L3 cache.