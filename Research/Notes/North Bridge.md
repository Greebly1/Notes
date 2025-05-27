A #Legacy computer hardware controller chip.

The north bridge received physical bit lines from the front side bus of a CPU AKA the [[System Bus]].

High performance / Critical external devices, like GPUs and RAM connected to the North Bridge.
	The North Bridge was primarily for the highest performance devices.

# [[Southbridge]]
Slower less critical devices such as HDDs, and audio devices **that still need data from the front side bus** would be routed through the North Bridge, then to a controller chip called the South Bridge.

# Memory Controller
The North Bridge in addition also handled the control signals and memory control of the DRAM.

# Modern Systems
As high performance external devices (GPUs, and RAM) needed increasingly more control communication to the CPU (Especially with the advent of DDR Ram), the North Bridge became absorbed into the CPU.

In modern systems, the GPU connects directly to the CPU Socket through dedicated PCIe lanes.
And DDR Ram now communicates directly to the CPU through Column and Row busses. 