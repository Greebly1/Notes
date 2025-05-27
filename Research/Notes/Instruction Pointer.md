[[Registers]]

Also called *Program Counter*

A special CPU register that stores a pointer to the next instruction for the CPU to execute.

**Cannot be directly written to**
	Only special control flow commands can write to the Instruction Pointer

# Control Flow
After each instruction, the instruction pointer will be incremented to point to the next instruction in line

Other instructions can modify the pointer
**JMP** - jump to
	Directly jumps to a new area in memory
	Used for loops
**CALL** - Function call
	Combination of saving return address, and jumping to area in memory
**RET** - Return
	Pops a value off the [[Stack]] (ideally a previous instruction pointer value) into the register
**INT** - Interrupt
	Triggers an interrupt handler program
**IRET** - Interrupt Return
	Return from an interrupt and restore the stack
**JCC** - Conditional Jump
	Jump to an area in memory if a condition is met

# [[Reset Vector]]
At the beginning, when a CPU is turning on, it will load the reset vector into the instruction pointer, signifying the start of the program and the first instruction for the CPU to execute.

