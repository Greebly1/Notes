[[TCP]] ports are virtual ports for different higher-level communication protocols built-atop TCP to use to differentiate each other.

It also allows multiple connections to be established

A port is literally just a number
	a 16 bit unsigned integer
	Ranging from 0-65535

# Well-Known Ports
Ports 0-1023 are registered for well-known protocols

| Port | Protocol   | Purpose                                |
| ---- | ---------- | -------------------------------------- |
| 20   | [[FTP]]    | Basic file transfer data               |
| 21   | [[FTP]]    | basic file transfer (control commands) |
| 22   | [[SSH]]    | secure remote host command access      |
| 23   | [[Telnet]] | Unsecure remote login to host          |
| 25   | [[SMTP]]   | Sending Email                          |
| 53   | [[DNS]]    | Finding IP addresses of domains        |
| 67   | [[DHCP]]   |                                        |
| 68   | [[DHCP]]   |                                        |
| 80   | [[HTTP]]   | Web traffic                            |
| 110  | [[POP]]    | Receiving Email legacy                 |
| 143  | [[IMAP]]   | Receive Email (modern)                 |
| 137  | [[NBT]]    | netbios over tcp                       |
| 138  | [[NBT]]    | netbios over tcp                       |
| 139  | [[NBT]]    | netbios over tcp                       |
| 389  | [[LDAP]]   |                                        |
| 443  | [[HTTPS]]  | Secure web traffic                     |
| 445  | [[SMB]]    |                                        |
| 993  | [[SIMAP]]  | secure IMAP                            |
| 3389 | [[RDP]]    | remote desktop access                  |
|      |            |                                        |

# Registered Ports
Ports 1024 – 49151 are for proprietary protocols, these can be registered with the [[IANA]]

# Ephemeral Ports
Ports 49152 – 65535 are for dynamic application use. You can use these to develop proprietary non-registered protocols.
This port space is mostly used after setting up a connection, the connection switches to some random ephemeral port and maintained.

Also used for security.

# Port Listening
If a port is *open* it means there is an application that is listening on that port for traffic.
	This is necessary for servers to remain available 

But it is important to understand the security concerns with having open ports.
	Especially when opening the well known ports

Threat actors constantly scan for open ports. In seconds they can determine all ports you have open, even ephemeral ports.