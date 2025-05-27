
A [[Malware]] type that remains undetected through one or more techniques.

For a virus to remain undetected, it may attach itself to the boot sector of a drive to avoid being found.

It may also hop from file a, to file b, both files managed by the malware but far away from each other in memory to avoid scans.

Malware that do this are referred to as stealth virus.

# Polymorphism
A technique by which a program changes its own code to evade detection.

An otherwise safe and useful piece of software may hide a complex hash key with malicious intent baked in that allows itself to alter its own instructions to avoid detection.

This is done with all instructions being dynamic. So it is very limiting.

# Root Kits
A technique where a virus alters the code of the OS somehow giving it kernel access and a perfect hiding spot.

# Fileless malware
Some viruses don't even have files stored on the computer except innocent looking binaries for storing state.
They achieve this once again by dynamically generating their instructions and deleting their executable when they are ran.
This way they live only on RAM
	The most famous fileless malware was [[STUXNET]]