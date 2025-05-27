Internet Message Access Protocol
Another [[Application Layer]] email retrieval protocol.

Intended to solve coherency issues with [[POP]]

# Email Coherency
Emails are stored in databases
	If you log in to your email on one device, retrieve an email, and instruct the database to delete that email, this device now owns the 'master copy' of the email. Good for security in case of data leaks
	However, if you log in to another device that has not downloaded that email, that device has no way of ever accessing the email that was deleted by your other device.

# IMAP Solution
IMAP works by keeping the master copy of the email on the database. The protocol works like a window into the database. you can view, delete, mark read, etc.

# Server Side
The IMAP server typically listens on Port 143
	However, secure IMAP (IMAPS) uses TLS/SSL on port 993

# Other Features
- Can partial fetch [[MIME]] data
- Message State data tied to an email (read, unread, replied, etc)
- Multiple mail boxes (folders)
- Server-side searches
- New-Mail notifications (not possible in POP)