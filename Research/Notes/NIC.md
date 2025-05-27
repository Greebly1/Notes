[[Link Layer]]

Network Interface Card/Controller

# Purpose
A NIC, controls the hardware involved with sending and receiving [[Physical Layer]] transmissions.
The main controller of a NIC is simply an [[Ethernet]] controller
	[[WIFI]] NICs use a WIFI controller chip (and may or may not include a dedicated [[Bluetooth]] controller chip) (some WIFI chips are dual purpose also performing Bluetooth)

A WIFI controller chip actually performs a altered version of the Ethernet protocol at the [[Link Layer]]

Also may utilize [[Fiber Optics]]
# [[MAC Address]]
Typically every Ethernet controller corresponds to 1 Ethernet port. And each controller will have a MAC address engraved into its architecture.
	WIFI/Bluetooth Controllers will also have MAC addresses

The controller chip uses the MAC address for Link Layer protocols.

# [[PCIe]]
Modern NIC expansion cards use PCIe slots. 
However they may use one of two techniques to transfer data
	Programmed input/output (often combined with CPU polling)
	[[DMA]] (often combined with [[Interrupt Request]]s)

# [[TCP-IP Offload]]
A feature some NICs provide. Good for Data centers where CPUs are bottlenecked by the overhead of the entire network stack.

# System Messaging
A NIC's job is to also tell the CPU of the availability of data.
NICs may do this with one of two techniques
	[[Interrupt Request]]s
	Polling
