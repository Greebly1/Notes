AKA
	Small Computer Systems Interface

Not 'small' anymore

One of the first ways we had standardized storage
- Hard drives
- Optical storage devices
- Scanners
- Tape Drives
- CD ROM
One controller supports 8-16 devices daisy changed
	Modern ones can do thousands for mass storage data centers

# Daisy Chaining
![[SCSI.jpeg]]
The SCSI communication bus is daisy-chainable, which is how it can connect so many devices.
	However it requires configuration

# SCSI ID
Since each device shares the bus, each device needs a unique ID so the controller knows who it is talking to.
	Furthermore a terminating resistor is necessary to absorb the electrical current and dampen reflections.

Depending on the device, the SCSI ID is configurable through physical switches, an electrical header, or some other method.

# Interfaces
SCSI, has a lot of different interfaces. Out of every hard drive protocol it has the most interfaces.

# Serial Attached SCSI
[[SAS]] for short, is a modern revamp of SCSI that makes it serial instead of parallel. 
Furthermore it does not use a shared bus topology, but a direct link, similar to PCIe. This means SCSI ID is no longer needed for configuration.

Despite being such a different standard, SAS is still considered SCSI because at a software layer, it functions the same as regular SCSI.