A proxy server forwards network messages on behalf of another endpoint.
	Operates at the [[Notes/IP]] layer
# Uses
- Masks IP
	The proxy server uses its IP during network messages, not the IP of the endpoint it represents
- Cheap to set up proxy servers
- Cache's resources such as websites
- Logs what network requests are being made
- Can block certain outbound network requests
	For instance, you can block malware from inside a LAN from accessing a control center
	Basically has a built-in [[Fire Wall]]

# How to configure
Proxy servers are typically set up right at the entry or exit of a gateway to a [[LAN]].
	Forward proxies do not need much configuration, but reverse proxies do. Often they have their own scripting/programmable controls for routing incoming messages.

# Two Types
![[Forward Proxy]]

![[Reverse Proxy]]

