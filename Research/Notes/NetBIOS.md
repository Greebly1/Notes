A #legacy #api used for [[Session]] layer of the OSI stack.

network basic input output system

developed by #Microsoft before the internet as we know it existed.
Originally it was tied very closely to [[SMB]]
![[NBF]]


![[netbeui]]

# How it Works
Since it is a session layer, NetBIOS' job is to provide indexing and addressing of specific programs between endpoints.

![[NetBIOS Name]]

![[NBT]]

![[NBTX]]
# Services
Name Service
- Broadcasts the [[NetBIOS Name]] and some other data to the [[LAN]]
- Resolves name system requests, if someone asks for the IP address of my program's name I will tell them what it is
Connectionless Service
- Sends and listens for messages without care of data loss
Connection-Oriented Service
- Sends and listens for messages with acknowledgements that they are received