A powerful, well-connected computer running [[Windows Server]] can be the domain controller for a [[Windows Domain]]. 

This computer runs [[Active Directory]], and stores its database. It likely also directly controls many other resources such as network drives.

The domain controller server also functions as the [[KDC]] for Kerberos

# Managing a DC
A Domain Controller can be managed by either
- Logging directly into the windows server machine
- SSH, Telnet, etc
- Through any LAN device with [[RSAT]]