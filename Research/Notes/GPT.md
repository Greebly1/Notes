#GUID Partitioning Table
Global Unique ID Partitioning Table

The modern partitioning format. 

# TLDR
**Pros**
- Larger (can support drives over 2TB)
- More partitions (up to 128 partitions)
- Data integrity (GPT uses [[CRC]]s to check for corruption)
- Compatibility with [[UEFI]]
- The standard supports future extensions
Basically no other cons, it is just better than [[MBR]], of which it is intended to replace.
**Cons**
- Requires UEFI hardware
- OS must be compatible for booting and/or data drive compatibility

# ![[Protective MBR]]
# ![[Hybrid MBR]]


