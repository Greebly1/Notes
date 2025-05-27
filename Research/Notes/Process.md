A process is a single program being ran on one or more processors

A process has at least 1 [[Thread]]
	The Master Thread / Main Thread
	Created by the OS when the executable file is ran

A multithreaded process may have multiple threads that may or may not run on multiple processor cores simultaneously.

# [[Page Table]]
Each process (managed by the OS) has a page table that maps their virtual address space to a physical address space. 
	All threads share the same page table, thus they share the same address space.

Exception
	Some special circumstances allow for processes to share addresses for inter-process communication 