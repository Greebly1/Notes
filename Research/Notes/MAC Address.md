[[Link Layer]]
Media Access Control
	Also known as physical address in #networking

MAC Addresses are globally unique identifiers #GUID 

# Anatomy
48 bits long - MAC-48/ EUI-48
	2^48 possible numbers, 281 trillion possibilities
	Will run out of addresses before 2080
IEEE Encourages adoption of EUI-64
# Type
3 types
	Unicast
	Multicast 
	Broadcast

# Locality
Utilized in local area networks [[LAN]].
MAC Addresses are included in every ethernet frame so devices receiving data know who sent it, and devices know if a message is meant for them

# Find Your MAC Address
Windows
	CMD --> ipconfig /all
MAC
	System Settings --> Network --> Select Your Network --> Details --> Hardware
IOS
	Settings --> General --> About --> WIFI Access
Android
	Settings --> About Phone/Device --> Status/Hardware Information --> WIFI MAC Address