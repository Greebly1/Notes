File Transfer Protocol
A connection-oriented #Protocol used to transfer files over a #Network. 

It is the language that computers speak in, to transfer files over a connection.

# Architecture
Uses a client-server architecture
FTP client software allows users to connect to a remote FTP server using TCP/IP.
	The FTP server is listening on [[TCP Port]] 21
Then the FTP client can issue commands to download (GETS), upload (PUTS), rename, move, etc.

Actual data transmission happens on TCP port 20.

# How to use
There are several ways to use FTP
Web Browser
	ftp.example.com (instead of http.example.com)
FTP Client
	Software the allows you to connect to an FTP server
	Most popular free FTP client (Filezilla)![[FTPClient.png]]
Windows shared folders
	Perform FTP on the backend automatically

# Extensions
[[SFTP]]
	Adds security and encryption
[[TFTP]]
	Simpler form of FTP that uses unencrypted UDP over a LAN