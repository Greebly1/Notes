Programmable [[Interrupt Controller]]

PICs, were very often separate chips entirely. 

whereas a CPU would have a single interrupt line (and by virtue a single main interrupt handler), a PIC would have 8 or 16 IRQ lines.

# Latching
The PIC would 'latch' the interrupt values and save them to poll-able registers that are mapped to memory addresses and readable by the CPU through its address bus, data bus, and RW line.

If any device asserts an interrupt on any of the IRQ lines of the PIC, the PIC would assert the CPUs Interrupt line.

# Multi-Mode
This also means that multiple devices can assert interrupts at the same time, even if they are on separate IRQ lines of the PIC. The CPU needs a way to determine which device is actually asserting the interrupt causing the PIC to notify its one single interrupt line

# CPU Side
The PIC contains data registers typically mapped to the CPUs data bus. 
The CPU's interrupt handler will read the register to determine which device is asserting and interrupt, then it will switch to the correct subroutine to handle it.
If the interrupt is still going, it will continue until all interrupts are gone.

# Cons
- Did not support multi-core processors
- Small amount of total IRQ lines (max of about 15)
- No load balancing or prioritization
- Slow I/O communication
