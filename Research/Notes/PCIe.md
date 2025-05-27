Peripheral Component Interconnect Express
	high-speed #serial expansion bus standard used to connect various #hardware components to a computer’s motherboard

Designed to replace [[PCI]] 

# Lanes
PCIe channels are broken into lanes
	x1 (by 1)
	x2 (by 2)
	x4 (by 4)
	x8 (by 8)
	x16 (by 16)
	x32 (by 32)
A PCIe channel is essentially a [[Expansion Slot]] standard for PCIe devices

A lane consists of a 2 pairs of wires
	Send pair
		Positive wire
		Negative wire
	Receive pair
		Positive wire
		Negative wire

Uses [[Differential Signaling]] to improve data reliability

Successful PCIe implementation requires top of the line conductors to be used in the lanes, as well as every wire pair to have less than 5mm of length disparity.
	Careful testing is also done to confirm the resistance of each wire is very similar, affected by the guage consistency and the turns in the wire path.
Failure to do these will result in extra reflectance, and signal timing mismatches.

# Clock and Data Recovery #CDR
The clock speed of individual bits in a transfer is interpreted by the edge transitions of the data transfer over the wires. At the receiving end a CDR circuit operates a loop (a phase locked loop PLL) (basically a redstone clock) that adjusts itself to the edge transitions of the receiving data.

What if the edge never transitions? 00000000 or 11111111? how does the PLL stay in synch?
# Line Coding
PCIe utilized #LineCoding, a technique where extra bits are inserted that are ignored however, they are set dynamically to ensure there are consistent edge transitions.

In addition this also improves the duty cycle, ensuring the transmission line is always close to 50% duty cycle.
	This is so the voltage does not drift too far up or down.

The specific encoding system used affects the efficiency.
8b/10b has 20% wasted bits.

# CPU Communication
PCIe slots may connect to the CPU
	1 Directly (faster) for GPUs and primary SSDs
	2 Through chipset (slower)

MOBOs can have multiple GPU slots by multiplexing a single PCIex16 channel.

# PCIe Versions
PCIe dynamically determines the lowest supported version to use

| Version | x1 Lane Bandwidth | Encoding  | Other                    |
| ------- | ----------------- | --------- | ------------------------ |
| 1.0     | 250 MB/s          | 8b/10b    |                          |
| 2.0     | 500 MB/s          | 8b/10b    |                          |
| 3.0     | 1 GB/s            | 128b/130b |                          |
| 4.0     | 2 GB/s            | 128b/130b |                          |
| 5.0     | 4 GB/s            | 128b/130b | NZR Signaling            |
| 6.0     | 8 GB/s            | PAM4      | Forward Error Correction |
