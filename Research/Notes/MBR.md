Master Boot Record

The first partitioning format. Uses [[LBA]] blocks, aka [[Sectors]], to create partitions of different types

MBR is the partitioning format that [[BIOS]] expects

Now considered #Legacy, it has been replaced by [[GPT]]
	It is however, more compatible especially for bootable drives.

# Sector 0
The first sector of an MBR drive is called the Master Boot Record

It contains a massive, complex data structure read by [[BIOS]] and the OS that tells them where the partitions are.
In this data structure is the partition table. It has
	4 slots for primary partitions
# ![[Primary Partitions]]

# ![[Bootstrap]]

# ![[Extended Partition]]


