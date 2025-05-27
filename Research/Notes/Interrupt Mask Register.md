[[Legacy PIC]]

The bit-width of the interrupt mask register will correspond to the number of IRQ lines.

Like any mask, an IRQ mask enables and disables IRQ lines from a programmable interrupt controller.

11111111
Enables all 8 IRQ lines on a PIC with 8 IRQ lines

00000001
Disables all IRQ lines except IRQ0.

When a line is disabled, even if a device asserts an interrupt to that line, the PIC will ignore it and it won't raise an interrupt to the CPU.

# Why
1. **Prevent low-priority interrupts from interfering** with high-priority tasks.
2. **Temporarily disable an interrupt while handling a time-critical section** in software.
3. **Disable malfunctioning hardware** that’s generating excessive interrupts.
4. **Enable or disable specific devices dynamically** based on system state.