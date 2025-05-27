Secure SHell

Developed for [[Unix]] systems as a replacement for [[Telnet]] and [[RSH]]


# ![[SFTP]]

# How to use
First of all, the server you are connecting to needs to
1. Be online
2. Use an SSH server program to listen on port 22

SSH as a client tool is used by simply starting a connection to a server via a single command
From that point forward, until the connection is terminated, all terminal commands will be forwarded to the remote server and executed there
	Command output (text, data, etc) will be piped back to your local shell automatically

The command is

SSH username@serverhost
	serverhost can be a domain name (example.com) or an IP address
		A domain name will perform a [[DNS]] query on the backend

Then you will be prompted for a password, the typing will be hidden

ex:

	SSH greebly@example.com
	assword

You are now in a secure shell

# Users and Passwords
When the SSH server is configured, users can be created and given different permissions.

This ties into Unix system permissions 

# SSH-keygen
Allows you to make a key instead of a password
This is useful for writing automation scripts
	You don't want to put your password into a script to access SSH


# SCP
Secure copy
Takes a local copy of a file and sends it to the server over SSH