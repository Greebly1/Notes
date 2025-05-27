An enterprise Hard drive interface designed to supply 4 PCIe lanes to hard drives directly, allowing for NVMe to be used.

It uses either 4 PCIe lanes, or two SATA links.

Primarily it connects SSDs through NVMe, but it also allows for SATA drives
![[U2Slot.jpeg]]
# Hot Swapping
 ![[Hot Swap]]
The U.2 interface supports hot swapping. Before U.2, data centers may have used M.2 slots, which are not hot swappable.
This makes maintenance difficult, since the server must be shut down to be repaired.
Data centers that used SATA were still hot swappable, however did not leverage NVMe
This is why U.2 exists, as a more scalable hotswappable form of m.2.

# Form Factor
U.2 drives fit the 2.5in form factor that SATA fit.
This form factor, compared to its cousin, the M.2, allows U.2 to get much much higher capacity.
The larger form factor also allows them to have better cooling.

# As an Interface
U.2 is an *interface*, not just a drive type. A storage server backplane determines what protocol is used
- SATA
- SAS
- PCIe (NVMe)
- Tri-Mode ([[U.3]])
This means a SATA drive might use the U.2 interface. SATA U.2 and SAS U.2 look identical.
Doing it this way makes it easier for manufacturers to make a single interface.
![[U2Interfaces.png]]
# Capacity
Consumer grade U.2s are common up to 4-8TB
Enterprise U.2 may reach up to 30TB
A single U.2 drive may actually be several SSDs striped together for performace.

# Replaced
U.2 as a standard is considered legacy now, since 2.5in form factor is a holdover from previous disk drives. 

The new standard to replace U.2 as the de-facto enterprise standard is 
[[EDSFF]]

# Adapters
U.2 adapters exist cheaply for m.2 slots, and PCIe slots.
	These often double as RAID controllers or HBA controllers

Additionally, some SATA ports may also support U.2.
	Check the PCB manufacturer

# Cons
- U.2 Drives are expensive
	- Often only sold in mass
	- More expensive per TB than M.2
- You need a very powerful CPU to be able to adequately use the performance boost
- MOBOs with U.2 are rare and expensive

# [[U.3]]
A special interface built from U.2
Does not increase speed but increases compatibility