Usually fragmentation occurs in [[Heap]] memory structures. However it can also exist on a [[Stack]], (both the hardware and/or virtual stack).

If we allocate memory objects to our memory map, at first we are using the space perfectly well, however over time those old memory objects are no longer useful to the program, so they will be freed.

When this happens the memory map becomes fragmented

![[BasicFragmentation.png]]

# ![[Types of Fragmentation]]