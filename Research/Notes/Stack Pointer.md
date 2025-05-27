[[Registers]]

Stack Pointer - (SP)

A special register that manages the [[Stack]]

**Can be directly written to**

	mov rsp, 0x7FFFFFFF ; Set stack pointer manually (unsafe if misused)

# Instructions

**PUSH** 
	put a value in a register on top of the stack, then increment the SP by the width of the sending register
**POP**
	Remove a value from the top of the stack, then decrement the SP by the width of the receiving register
**CALL**
	PUSH the current value in the [[Instruction Pointer]] to the stack
**RET**
	POP the top of the stack into the [[Instruction Pointer]]

# SP Arithmetic
Often read from to perform math to determine how far down the stack certain values that we know are.
