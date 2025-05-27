A thread is the lowest unit of a program.

It represents its own instructions, and is context switched as if it is a program.

Every [[Process]] has at least 1 thread
	This is the master thread or main thread

# Memory and Resources
All threads share the same memory.

They all belong to the same process so they are treated the same.
	Each thread is context switched with the page table of its process. Meaning it can access the same memory as other threads in the same process.