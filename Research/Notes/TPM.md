Trusted Platform Module
A hardware encryption chip the improves security by adding special hardware-backed keys and encryption decryption tools.

Software utilizing a TPM can take their encryption keys, give it to the TPM and ask the TPM to encrypt them using a globally unique hash burned into the TPM by the manufacturer.

# TPM Root Key
A hash key burned into a TPM by a manufacturer
It cannot be read or derived.

# Key Wrapping
Application level encryption keys can be encrypted by the TPM with its Root Key then safely saved to disk or ram. 

When the key needs to be used again, the TPM can unwrap it for the application.
# Key Sealing
Additional data is baked into the wrapping of the key, the register values must be the same to prove that the environment has not changed.

The environment is all of the platform configuration registers. Set during boot.

# Hardware Certificates
The TPM also stores certificates that cannot be read. 
The certificates use special hashes to prove a binary is the same as the original equipment manufacturer.

# Hardware Acceleration
The TPM can do certain cryptographic functions faster than the CPU.

# Connection
TPM uses either a proprietary connection bus, or a low pin count [[SPI]] bus.