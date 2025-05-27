
**Stale Cache**
	Cache that is too old may no longer represent what that value actually is. Especially in MMIO

Some cache systems utilize a [[MESI]], that contains extra data for each cache entry denoting if it is valid or not.

# [[Non-Cacheable Memory]]
Some memory is inherently always going to be invalid if in a cache. For instance, MMIO.

Its just safer to never cache these values, always do a full read for data reliability and precision.

# Multiprocessor Systems
In systems that implement multiple processors and thus multiple caches, a cache coherence policy should also ensure that all caches know the state of other caches.

For instance, if two private caches contain the same value, but one processor writes to one cache, the other cache should be notified somehow that the memory they contain is no longer valid. It is stale.