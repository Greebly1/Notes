In some [[RAID]] systems, you can nest RAID implementations within single drives of a greater RAID system.

Typically this is only done with two layers, a top controller and (several) child controllers each with their own RAID levels and independent configurations. 

RAID 1+0 (RAID 10)
- [[Striping]] an array of [[RAID 0]] [[Mirroring]] drives.
- There exists a special form of software RAID 10 developed for Linux that performs better by using intelligent optimizations.

RAID N+N (JBOD) (Just a Bunch Of Disks)
- A special non standard form of RAID that allows for concatenating disks and full RAID arrays.

Enterprise systems may use  a very complex nested RAID hierarchy that ensures maximal performance and data reliability.