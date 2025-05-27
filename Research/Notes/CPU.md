Central Processing Unit

The CPU executes instructions made by a programmer, and defined by the CPU's [[ISA]] (Instruction Set Architecture)

# Registers
Instructions are performed on, and with [[Registers]], which serve as the working memory of a CPU.
	A register is like a CPU's hand, it can hold things and do things with what it is holding.

# Socket
Various specifications and features of a CPU are standardized into a [[CPU Socket]] which operates as the interface between the CPU and the rest of the computer.
	[[ISA]]
	Registers
	Clock speeds
	Supporting peripherals
	External address bus
	[[Memory Controller]]

# [[CPU Cache]]
Reading data from #RAM is actually very slow relative to the CPU time scale.
Modern CPUs have a #Memory-Hierarchy with fastest memory at the top.
Cache is a small amount of memory inside the CPU that saves values that are repeatedly used so the CPU does not need to continuously fetch them.
![[MemHierarchy.png]]

# [[Memory Controller]]
The CPU must be able to communicate with the rest of the computer using memory addresses. 
Modern CPUs contain a MMU (memory manager unit), that handles communication through the external data bus.
	It also performs modern features such as virtual memory, Memory Mapped IO, etc.

# Control Unit
A macro controller for the entire CPU. Controls and coordinates all the different units.

# [[Clock Rate]]
CPUs utilize a electronic clock, like a red stone clock that signals to the entire CPU when to move forward like a drummer. 

Naturally, faster clocks cause faster execution. A CPU though, can only support a maximum given clock rate before it starts to fall apart and miss critical timings.

# Heating
CPUs produce an incredible amount of heat, especially when the clock rate is high.
#TODO


# Arithmetic Logic Unit ALU
A unit designed to perform a set of specific arithmetic operations on general purpose registers using whole number integer binary representation

# Floating Point Unit FPLU
A special Arithmetic Logic Unit that performs fractional arithmetic operations using floating point binary representation.

# Address Generation Unit
A arithmetic logic unit optimized for pointer arithmetic.

