
Some [[NIC]]s have a small ARM/MIPS processor and memory that can package and unpackage TCP/IP messages.
	This takes a lot of load off of the Main [[CPU]] especially in data center speed ethernet controllers.

Some implementations use field programmable gate arrays #FPGA  alongside a processor.
Some implementations also allow for **user-space network control programs** (which intercept network operations usually performed by the kernel) to be loaded ran on the processor such as Solarflare's #open-source **OpenOnload** network stack used by Linux.

