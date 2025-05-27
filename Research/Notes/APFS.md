#Apple [[File System]]

The modern next-generation file system for Apple platforms. Intended to replace [[HFS+]]. in fact HFS+ partitions can be reformatted into APFS by disk utility.


# Space Sharing
APFS partitions have a unique feature that allows them to dynamically grow and shrink to meet memory demands. If you have two partitions on a drive, and the platform detects that one volume is being used a lot more and is close to overfilling, it will dynamically repartition the space to give it more share of memory.
Partitions can also grow to fill empty unpartitioned space

# Copy on Write
![[COW]]

# Atomic Safe-Save
![[Atomic Safe-Save]]
