New Technology File System

A #proprietary  file system released alongside [[WindowsNT]] in 1993

It is the de-facto standard [[File System]] for [[Windows]]

# TLDR
## Pros
- Scalability
	Practical limit of drive size (256TB)
	Theoretical limit (16 exabyte)
- [[Journaling]]
- Compression
- Encryption
- Permissions
- Resizing
- Quotas
	This user gets to use blank amount of space

# Compression
In NTFS, a [[Lossless Compression]] function can be used to compress files, and entire directories.
To do so, right click a file/directory and go to properties->advanced->compress

Doing so will change the name of the file to blue or add a compression icon

# Encryption
in the same way as you compress files you can also encrypt them. 
However a user can only encrypt files if the [[Windows Domain]] allows them to.

**You cannot encrypt and compress files at the same time with NTFS**

# ![[NTFS Permissions]]

# How it works
Way too fucking complicated
#TODO