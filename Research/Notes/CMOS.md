Complementary Metal-Oxide Semiconductor

CMOS stores configuration data for [[UEFI]], it stores BIOS settings

Typically a CMOS is two 64 byte memory banks, so 128 Bytes in total.

CMOS is volatile memory, so it must be powered at all times or it will be wiped
	Unpowered CMOS is actually just wiped to system defaults
# [[CMOS Battery]]
CMOS is powered by a lithium coin battery on the Motherboard. 

# CMOS Clear
A common practice when needing to reset CMOS, such as being locked out because of a forgotten bios password is to simply clear CMOS

There are multiple ways to do this, either a built-in CMOS clear wire, CLRK on the motherboard can be jumped, or the CMOS battery can be removed and time will drain the remaining voltage.
