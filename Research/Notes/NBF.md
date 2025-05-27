# NetBIOS Frames
[[NetBIOS]] that ran over [[IEEE 802.2]], predates TCP and UDP. Developed by #Microsoft for their early [[SMB1]] systems for [[DOS]] networking. 

During this ancient time NetBIOS and 802.2 was how LAN devices communicated.

Essentially the netbios handler's job is to route messaged to the correct internal program using the message's Netbios name.
Back then the 802.2 network handler sniffed for LAN frames that contained a bit signalling that it was for netbios. 