Simple Mail Transfer Protocol

Used for sending [[Email]] to a mail server
A connection-oriented text based TCP main sending protocol

# Terminology
A Mail User Agent (MUA) sends mail to a mail submission agent (MSA), which may forward the mail to a Mail Transfer Agent (MTA) to a database that also runs a Mail Delivery Agent (MDA)

# Server side
SMTP servers typically listen on port 25, however some spam filtered servers listen on port 587 (previously 465)

# Local SMTP (LSMTP)
For forwarding mail within a network. A mail delivery agent or storage agent can use LSMTP when within a network.
Common in very large organizations
Adds more security by requiring users to already be authenticated by the network.