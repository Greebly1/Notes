A #broadcast-domain is a collection of connected devices (a network) where all devices can hear broadcasts from all other devices, and vice versa.
[[Hubs]] and [[Switches]] forward broadcasts, meaning everything connected to one of their ports is in their broadcast domain.
[[Routers]] do not forward broadcasts.

A [[LAN]] is a broadcast domain

Most cellular and wireless networks are also broadcast domains

# Contention
Small broadcast domains are great, however extremely large broadcast domains, hundreds of thousands of devices, will slow down the network.

So network administrators commonly segment giant broadcast domains into smaller ones using [[Routers]].
- The workstation floor
- The main office
- etc