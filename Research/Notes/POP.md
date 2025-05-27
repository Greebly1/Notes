Post-Office Protocol

The most common [[Email]] retrieval protocol used today.

Exists at the [[Application Layer]], by applications to retrieve emails from a server

# Retrieve and Delete
POP allows the client to both retrieve mail from a mail server and delete the mail off that mail server.

Often received mail is downloaded and saved onto the client computer

Deleted mail is often just marked as deleted, but stays in the mail database

# Server-Side
A POP3 server listens on [[TCP Port]] 110 for connection requests and commands.
A secure POP3 server may listen on port 995

# Versions
POP is synonymous with POP3
However other versions and extensions exist
	POP3S
		A secure version of POP3 that sets up an initial encrypted connection using [[TLS]] or [[SSL]] on port 995
	STARTTLS
		Extension that lets clients use TLS or SSL security using a new STLS command, or instead by using port 995
	SDPS
		Standard Dialup POP3 Service allows users to access multiple virtual accounts using the same credentials. Used extensively by Google.
	KPOP
		Special secure version of POP3 encapsulated in the Kerberos security protocol