[[CPU]]

The top of the memory hierarchy.

Registers are the working memory locations that are used when performing arithmetic and comparison instructions as well as load and store instructions. 

The register involved in an instruction is built into the instruction itself.

# Register Width
Over the years registers have changed sizes, for new CPUs to support backwards compatibility for older programs, larger registers have historically just been extensions of the smaller registers.
![[RAX.png]]
An instruction
	MOV RAX 0xFF00; moves 64 bits into RAX starting from address 0xFF00
But
	MOV AL 0xFF00; moves 8 bits into AL starting from address 0xFF00

# Types
There are many types of registers
Hardware Registers
	registers on external devices, indirectly accessible
Control Registers
	Used to set the behavior of the CPU and features
Address Registers
	Used to store memory addresses
General Purpose Registers
	Used for instructions such as the RAX register
Status Registers
	Hold 'truth' values resulting from previous comparisons
Constant Registers
	Hold hard coded values such as PI, TAU, e, etc
Special Purpose Registers #SPR
	Used for specific control purposes such as the instruction pointer
Model-Specific Registers
	Store information about the CPU model
