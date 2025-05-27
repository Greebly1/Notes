The chipset was once a myriad of device controllers on a MOBO. Today a single chip, the Platform Controller Hub (PCH) performs the responsibilities of all the chips combined.

# Multiplexing Devices
A CPU only has so many pins for I/O, but a computer may have any number of connected devices, expansion slots, and peripherals.
	Modern CPUs call these pins the [[DMI]] pins

The PCH works as an I/O multiplexer and translator between CPU and the many devices connected

# Bridging
Furthermore, the PCH also works as a protocol bridge, translating between multiple protocols.
	[[PCIe]]
	[[SATA]]
	[[USB]]
	HDAudio
	Etc
This allows the CPU to communicate to unique communication protocols through a common language.

# Bandwidth Arbitration
Since many devices share the few [[DMI]] pins, the PCH is in charge of prioritizing bandwidth so that all devices get a chance to communicate, and important devices are not overshadowed by many less important ones.

# Extra Features
Firmware-based security
- Intel PTT
- AMD PSP
Overclocking Controls
[[RAID]] Controllers
Sometimes embedded memory and cache controllers
