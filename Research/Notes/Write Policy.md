
How a cache system handles writing to memory that is also saved in cache.

Furthermore, systems with a cache hierarchy, need to notify all caches of a write.

# Write-Through
Every write to cache causes a write to main memory

# Write-Back / Copy-Back
Writes to the cache, and marks them as 'dirty' requiring an eventual write.
	At some point all cache marked 'dirty' is written to main memory in bulk
This is often called the [[MESI]]

