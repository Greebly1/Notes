A checksum is a technique used to detect if an incoming network message is corrupted.
	Corruption may be caused by a malicious user spoofing things, or just unreliable network segments with bad signal retention.

# How it works
Checksums first need to be calculated before sending a message.

**Checksum Algorithm**
1. Add all the bytes together (don't worry about integer overflow) (potentially just use a 64 bit unsigned integer)
2. Take the last byte of that sum and append it to the end of the message.

When the packet reaches the destination address the endpoint will do the same checksum algorithm and check if the two checksums match.
	If they do not match then the data is unreliable, maybe a bit was flipped or dropped along a bad network segment.

# Cons
Calculating a checksum for every message adds extra overhead

Oftentimes multiple checksums are 'tunneled' within each other, adding wasteful calculations.

Does not guarantee message was not tampered with.
	Middlemen can simply change a message, and recalculate a new checksum. 
	Checksums are ONLY used to determine if a message is corrupted or not