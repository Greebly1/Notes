AKA
	Fetch-Execute Cycle
	Instruction Cycle
	CPU Cycle

Ignoring Interrupts

The instruction cycle is the process that a processor follows when executing a program.

# Fetch
The CPU reads 1 byte from memory at the address that the [[Instruction Pointer]] points to. Then it increments the instruction pointer
	This is the instruction in assembly, Ex: ADD AX __address__
		In reality it is just a bunch of numbers that we all agree, means ADD AX
# Decode
The CPU decodes the instruction bits, and determines what operations need to be done to execute the command.
	This is what the instruction means, EX: the next 64 bits are a memory address.
	Read the next 64 bits
	Increment the instruction pointer
	Interpreting those bits as an address starting point, fetch the next 32 bits from that address offset in memory
	Add those 32 bits retrieved into the AX register

# Execute
The CPU performs the instruction by doing one or more operations

