AKA
	Redundant Array of Inexpensive/Independent Disks

RAID is a data storage virtualization technique that aims to improve data reliability and/or read/write speeds. 

# RAID Levels
Data is spread across multiple drives (an array of drives) and accessed in accordance to a RAID Level, that provides data reliability and performance benefits.
-  ![[RAID 0]]
-  ![[RAID 1]]
-  ![[RAID 2]]
-  ![[RAID 3]]
-  ![[RAID 4]]
-  ![[RAID 5]]
-  ![[RAID 6]]
# [[Nested RAID]]
In addition to the RAID levels, some systems leverage specific techniques between RAID levels. 

# Implementation
RAID may be implemented in one of two ways
Hardware [[RAID Controller]]
- Processing offload, (useful for #Enterprise servers)
- Some experts warn against modern hardware raid for data reliability

[[Software RAID]]
- More CPU load
- Greater flexibility and control

In all cases, you will need anywhere from 3-3000 hard drives in order to make a useful RAID implementation