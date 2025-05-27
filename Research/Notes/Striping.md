A special form of [[Drive Concatenation]] used in [[RAID]] where instead of appending the start of one drive to the end of another drive, memory addresses are interleaved between all drives.

Doing this improves write and read throughput.

# Stripe width
Striping can be done with different sizes of data. For instance
- Stripe each bit
- Stripe each byte
- Stripe each word
- Stripe each block

Each has different benefits and drawbacks. For instance, striping each block improves the latency of small reads, but doesn’t have as good overall throughout.

However, striping each block tends to be the modern best method, since modern drives read entire blocks at a time anyways. So actually, it has the best throughput.