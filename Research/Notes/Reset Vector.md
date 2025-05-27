
When a CPU is powered and it has finished its restart sequence, it will perform a read from a specific memory address defined by its [[ISA]], and load the value into the [[Instruction Pointer]] register.

The reset vector is provided by the [[Flash ROM]] on the MOBO. It points to the beginning of the [[UEFI]] / [[BIOS]] program often in the same ROM chip. 