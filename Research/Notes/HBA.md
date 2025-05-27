Host bus adapter.

A type of expansion device that allows for the adding a multitude of hard drives. 
This allows motherboards to be upgraded to support much, much more storage.
# How
HBAs typically (slotted to a PCIe slot) use the [[PCIe]] protocol to create its own PCIe device hierarchy which it reports back to the CPU as individual devices.

A HBA controller essentially provides a system bus to all of its local devices by forwarding PCIe messages to the correct device, or by translating between protocols and routing messages between the CPU and the devices.

# Protocols
HBAs may use [[SCSI]] daisy chaining, it may use [[SATAe]], it may simply forward PCIe messages (in the case of [[NVMe]].

HBAs may even support more than one protocol, such as ![[Tri-Mode]] storage interfaces.

# [[RAID Controller]]
A special type of HBA that appears to the CPU as a single device, but performs all the necessary algorithms to support RAID.