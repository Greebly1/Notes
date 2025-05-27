Server Message Block
A #Network #Protocol 
AKA
	CIFS - Common Internet File System

# Features
- File Sharing
- Printer Sharing
- Network Browsing
	Allows clients to discover available SMB services
- Access Control
	Robust controls for administrators to configure server permissions and resource access
- Opportunistic Locking
	Performance improvement by caching file data
- Message Signing
	Ensures authenticity of messages
- Encryption
# Architecture
Client-->Server model
	Client: 
		connects to server, 
	Server: 
		listens on ports and respond to requests

Uses Sessions to track connections

# Protocol
**1 Session Establishment**
	Client requests a session via a transport protocol (often via [[NetBIOS]] for legacy)
	Server responds, establishing a session
**2 Authentication**
	Client sends auth credentials
	Server grants or blocks access
**3 Resource Access**
	Client requests access to a resource (file, printer, etc)
	Server checks permissions, grants them
**4 Data Transfer**
	Client & server exchange data/commands to modify or transport the resource
	Data is transferred with encrypted SMB packets
**5 Session Termination**
	Client requests to close a session
	Server responds
# Versions
![[SMB1]]
![[SMB2]]
[[SMB3]]

# Uses
**Corporate Networks and SOHO**
- Efficient file sharing between workstations
- Streamlined access to printers
**Educational Institutions**
- Provides access to shared resources
- Configuration controls for permissions
**Data Centers**
- Storage access and management for large scale virtualized systems
**Media Streaming Applications**
- Direct connection to SMB server for direct streaming of media

# Implementing
**Set up SMB Server**
- Enable "File and Printer Sharing" on Windows
- Or install SMB software
- Or create a shared folder (Windows)
**Configuring SMB Clients**
- Map network drives
- or set up network locations for files and printers
**Maintenence and Security**
- Implement authentication and permissions for resources
- Regularly update SMB software
- Monitor SMB errors