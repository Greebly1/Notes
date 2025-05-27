Virtual [[File System]]

A #Linux file system #abstraction layer. 

![[VFS.png]]

When a disk operation is required by the kernel, it routes the request to VFS, which keeps a map of memory ranges to file systems. It decides what file system driver to route read requests to.