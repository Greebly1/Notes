(IPI)
Also known as a '*shoulder tap*'

A special low level [[Interrupt Request]] in #Multi-Core systems where one processor can interrupt another processor if it requires specific actions to be done.

# Why?
- flushes of [memory management unit](https://en.wikipedia.org/wiki/Memory_management_unit "Memory management unit") caches, such as [translation lookaside buffers](https://en.wikipedia.org/wiki/Translation_lookaside_buffer "Translation lookaside buffer"), on other processors when memory mappings are changed by one processor;
- stopping when the system is being shut down by one processor.
- Notify a processor that higher priority work is available.
- Notify a processor of work that cannot be done on all processors due to weird proprietary micro architectures
- An OS scheduler may want to handoff a specific thread to a core.

# Interrupt Request Level [[IRQL]]
IPIs have an IRQL of 29