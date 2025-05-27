
A stack is a Last-In-First-Out #LIFO data structure that lives in [[DRAM]].

The stack stores data **whose size is constant**. Most commonly, pointers to the [[Heap]], or temporary register values.

# How to Use
Stacks like any #LIFO, is used with PUSH, POP, and LOAD commands.
PUSH
	Put a value on top of the stack, and increment the [[Stack Pointer]] by the bit width of the value
POP
	Read and remove an item off the top of the stack, and decrement the [[Stack Pointer]] by the width of the value
LOAD
	Since the stack is just a memory location, you can read the current stack pointer, and perform pointer arithmetic to read any value on the stack, for instance read the 4th value down the stack without POPPING it.

# Locality
"Every [[Thread]] has its own stack"
Where a process' stack is in [[DRAM]] is determined by that process' [[Stack Pointer]]. The max size of any stack is defined by the OS' process memory allocation, and enforced using #page-faults. 

# Kernel Stacks
"Every [[Thread]] actually has 2 stacks"
One stack for #User-Mode and one stack for #Kernel-Mode

# [[Context Switch]]
A stack is one of the many things that is swapped out when the OS performs a context switch on a processor/