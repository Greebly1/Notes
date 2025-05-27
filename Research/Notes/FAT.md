File Allocation Table

A very old [[File System]] and [[Hard Drive Format]] originally made for [[MS-DOS]] in 1977 for [[Floppy Disk]]s

It is still commonly used on external drives such as [[Flash Drive]]s and [[External SSD]]s. This is because being the oldest format and file system, it is the most compatible when moved between platforms and operating systems.

# Pros
- can be used with any platform or OS
# Cons
- Slow
- Max file size is 4gb (unless using [[exFAT]])
- No permissions
- No encryption
- No low level compression
- Doesn't support journaling


# How it works
A file is
	A linked list of blocks
	
Unlike a linked list, each entry **does not** include a pointer to the next entry
	This is the purpose of the **file allocation table**

**FAT**
	A table that is indexed by block number, and contains a pointer to the next block or, -1 which denotes end of file.
	It also stores a single bit entry, for whether a file is empty or not
ex

| Index | Busy (empty) | Next | notes       |
| ----- | ------------ | ---- | ----------- |
| 0     | 0            |      |             |
| 1     | 1            | -1   | end of file |
| 2     | 1            | 3    |             |
| 3     | 1            | 4    |             |
| 4     | 1            | 5    |             |
| 5     | 1            | -1   | end of file |
| ...   | ...          | ...  |             |
FAT tells us how to glue blocks together into a file, and where a file ends, but it does not tell us where files start
	This is the job of the directory table
	Directories are also treated as files

Directory Table Format

| Filename | Starting block number | meta data |
| -------- | --------------------- | --------- |
The root file directory table is always at the same address so software knows where to start

Note: subsequent directory tables are stored inside blocks maintained by the FAT

# Types
Several types of FAT exist. Most of them simply change the block size. from 8 bit to more modern 32 or 64 bit
[[FAT8]]
[[FAT12]]
[[FAT16]]
[[FAT32]]
[[exFAT]]
	A special extension that allows the block size to be dynamically configurable to be as large as we want for the whole drive.
	Furthermore it can support files larger than 4gb
