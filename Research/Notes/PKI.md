Public Key Infrastructure

An infrastructure system designed to stop [[On-Path Attacks]] also known as Man-in-The-Middle attacks during a [[Key Exchange]].

# Problem
Client -- man in middle -- Server

If the client cannot verify that a public key is actually belonging to a server or a man in the middle, then the man in the middle can decrypt and re-encrypt a set of keys and eavesdrop, or worse.

# Solution
A third party will distribute public keys alongside identifying information about the owner of said public key, and a certificate proving they are who they say they are. All encrypted with the third party's private key as a certificate for the third party.

![[PKI.png]]

Both the sender and receiver have the [[CA]]'s public key, so man in the middle attacks do not work between a client and a CA.
The CA turns identifying information, as well as the sender's public key, and creates an encrypted digital signature that proves the CA has vetted it.

This is called a [[X.509]] certificate.