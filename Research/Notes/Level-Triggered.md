
The [[Interrupt Request]] is held continuously as long as the IRQ line is held below a certain point.

This standard expects that when the CPU decides to handle the interrupt, it will do something that will indirectly or directly cause the thing holding the IRQ line low to stop.

# Multi-Mode
In much older systems, a single physical IRQ line can be held down by several external devices, requiring the software interrupt handler to determine which device needs servicing.

If the interrupt line is still held down, then it will check the next device.

Often there would be a virtual IRQ table, so devices can register that they have indeed initiated an interrupt.
	The storage was often just a hardware latch managed by the CPU.