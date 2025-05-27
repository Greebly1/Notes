Extensible Authentication Protocol #EAP 
AKA - 802.1x
	- RFC 2284

A barebones #API used to authenticate users into a network. It doesn't implement any backend, only providing the message structure for different software handlers and devices to adhere to.

Created shortly after 2005 to solve the [[Hardware Addition Attack]]s by requiring devices to be authenticated by a central database managed by a security admin.
	Usually admins still provide a guest network access that is segmented off from the main network.

# Architecture
![[EAP.png]]
EAP mainly exists as a client-server API between a **Supplicant** (client device) and an **Authenticator** (Access point). The **Authentication Server** is the implemented backend

# Client Side 
In order to connect to EAP networks, client devices must run some kind of EAP handler in their network stack.
![[Client-Side EAP]]