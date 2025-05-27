A hardware device that functions as a smart [[HBA]].

A RAID Controller manages a large amount of Hard Drives, and performs the necessary routing, and parity instructions in order to group them into a [[RAID]] array.

As opposed to [[Software RAID]], a hardware controller helps offload parity and routing overhead that the CPU would otherwise need to manage.

## Single Device
A RAID controller, contrary to an HBA, appears to the CPU and OS as a single device, and usually doesn’t report its entire local device tree, since it manages it itself.

# HBA Mode
Many high end RAID controllers have a special option that allows them to operate like a normal HBA. Which means it will report each local device up the chain to the CPU to manage.

AKA IT Mode