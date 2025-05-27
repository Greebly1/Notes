[[Interrupt Controller]]
Interrupt Request (IRQ)

A special hardware signal sent to the [[CPU]] to suspend a running program to allow an [interrupt handler](https://en.wikipedia.org/wiki/Interrupt_handler "Interrupt handler"), to run instead. 
	used to handle events such as receiving data from a [[NIC]], key presses, or mouse movements.

**Interrupt Line**
an interrupt line corresponds to a device. It is the actual means for a device to send an IRQ to the CPU. The specific line allows the CPU to know which device the IRQ originated.

How many Interrupt Lines are available depend on the type of Programmable Interrupt Controller [[Interrupt Controller]] a CPU uses. 

# Line Types
**Physical**
	In older computers every interrupt line was a physical wire, typically going through the [[Southbridge]]
	For instance, a keyboard would send interrupts on IRQ Line 1 by 'pulling the line low' and lowering the voltage to signal
	The amount of interrupt lines connected to the CPU scaled with the number of devices a socket must support. Typically in powers of two.
**Logical** I/O
	
