A Motherboard that has more than 1 [[CPU Socket]]. Almost always for #Enterprise servers

![[MultisocketMOBO.jpg]]

# Hardware Implications
Each CPU actually has its own RAM slots. But they can still read and write to ram that doesn't belong to them, they simply need to go through a slower interconnect bus, such as [[Infinity Fabric]]

Extra robust cache coherency must ensure that cache memory is invalidated if the other CPU writes to that memory address.

# Software Implications
OS virtual memory systems try to keep physical memory given to a thread on one ram slot.

OS schedulers try to optimize by context switching into the CPU whose physical memory previously belonged to the thread they are switching.

Multi-core techniques already solve many problems in multi-socket computers. For instance synchronization between accessing shared data is already solved with OS primitives.

# Form Factor
Most server MOBOs are [[ATX]]. however many manufacturers make custom sizes that fit into their standardized server racks.
