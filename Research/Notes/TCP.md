Transmission Control Protocol

TCP is a connection oriented communication protocol built on top of [[Notes/IP]] internet protocol.

It solves the issues involved with sending communications via an inconsistent delivery service. 
	- Failed message deliveries
	- Delivered in wrong order

# Connections
TCP first establishes a connection between two hosts via the
![[TCP Handshake]]

If a connection drops (acknowledgment messages stop) another TCP re-handshake process will initiate.

# ![[TCP Port]]