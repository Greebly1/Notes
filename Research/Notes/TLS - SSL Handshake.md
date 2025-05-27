A series of messages used to turn a TCP connection made from the [[TCP Handshake]]
into a secure [[TLS]] or [[SSL]] connection.
![[SSLTLSHandshake.png]]

# #TODO
understand each message in the process

# 1. Client Hello
**Unencrypted**
**Client** --> **Server**
- TLS version
- Client random number (protects from [[Replay Attacks]])
- List of supported ciphers
- List of support compression schemes
- Protocol extensions
- [[ECDHE]] parameters (client's ephemeral public key)

# 2. Server Hello
**Unencrypted**
**Server** --> **Client**
- Chosen TLS version
- Server random number (protects from [[Replay Attacks]])
- Chosen cipher
- Session ID
- Server [[ECDHE]] (server ephemeral public key)
- Accepted extensions

# 3. Certificate
**Unencrypted**
**Server** --> **Client**
[[X.509]] Certificate Chain
- Includes server public key [[RSA]]
