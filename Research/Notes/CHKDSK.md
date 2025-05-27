Check disk

A [[Windows]] #command used to scan a drive for corruption or failed memory cells

**Considerations**

chkdsk can only be used with local [[Hard Drive]], it does not work with network mounted drives. 

chkdsk can only be performed by administrators 

You should try not to interrupt the command, however you can cancel it without causing issue

# Logical Check
At the software level chkdsk will check if the data structures are configured properly.
- Corrupt meta data
- Cross-linked files
- Conflicting memory allocations
- Lost clusters (data with no owner)

# Hardware Check
A hardware check is done using a standard hardware API. Bad sectors and blocks are marked in the software so they are not used.
	It also moves data from bad sectors to good sectors

# Options
-f
Attempts to fix problems it finds

Other options don’t really matter