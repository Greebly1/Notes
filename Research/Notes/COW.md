A File System optimization strategy whereby, copies of files point to the same memory address.
If a change is made to one of those copies, it save it as an incremental change to that specific file pointer.

![[COW.png]]

# Cloning
The act of copying a file pointer and meta data. The underlying data of the file is still unchanged and in the same location. But now there are two virtual files pointing to that memory.
In the case of COW, further changes to one of these clones saves at incremental changes.

# Snapshots
![[Snapshots]]