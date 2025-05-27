[[WiFi]]

This is the first protocol performed when connecting to a wireless network. It facilitates the discovery of networks, and the connection to them.
![[Association.jpeg]]
# 1 Scanning/Probing
**Passive Scanning**
	Wireless access point broadcasts **beacon frames** advertising itself, this information includes its name and SSID.
	Since certain devices mainly operate on one of the 3 frequency bands, some devices cannot see a WAP's beacon frames.
**Active Scanning**
	A wireless capable device can broadcast **probe requests**, asking any wireless access points in range for their name and SSID.
	WAPs that hear the probe request may respond with **probe responses**

If two devices do not both support the same EMF band, they simply cannot hear each other, and thus are unable to connect.
Otherwise, the network will appear as an available network from a network capable device.

# 2 Authentication
**Authentication Request**
	A device asks to be authenticated and/or to be associated with the network.
**Authentication Response**
	WAP responds with authentication requirements
	yes/no/password locked/etc

# 3 Association
**Association Request**
	Device provides a password attempt if password is required. Asking to join the network.
**Association Response**
	WAP accepts or declines the request to join the network.