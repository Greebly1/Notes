
Modern CPUs may adhere to a specific [[ISA]], but use that as an API to translate their own micro-architecture commands.

A single ISA instruction might be broken into hundreds of tiny microprocessor commands each with their own Opcode.

# [[Fetch Decode Execute]]
Part of the Decode process is determining what micro commands and Opcodes are needed for an ISA instruction. 

# Instruction Cache
With all this in mind, it is actually very beneficial for instruction Opcodes to be cached according to what ISA instruction they come from. This saves the CPU from reading from its list of opcodes to find the correct one.

Some [[L2 Cache]] might also be instruction caches.

# Loops
This is extra beneficial during algorithmic loops. Where the same instructions are performed over and over again.