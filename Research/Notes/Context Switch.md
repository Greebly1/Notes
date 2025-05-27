A context switch refers to the process of switching the data and registers inside a CPU core that have to do with one program with the data and registers that have to do with a different program.
	In effect the CPU has switched to an entirely new environment and is executing different instructions

The data involved in a context switch
	The [[Stack Pointer]]
	The [[Instruction Pointer]]
	The register values
	The [[Page Table]]
	Some cache stuff

All of this data is saved by the Operating system and associated with a process.

# Scheduling
Context switching is typically performed by the [[OS Scheduler]]