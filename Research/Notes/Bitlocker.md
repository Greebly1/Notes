#Microsoft  full drive encryption tool first introduced in [[Windows 10 Pro]]
	Note: it doesn't encrypt the boot sector, so the OS can still boot.

Bitlocker lives in the hidden [[Windows System Partition]]

It uses [[AES]] 256 for encryption/decryption

# Recovery Key
When bitlocker encrypts your drive it will prompt you to create a recovery key, which is a very large hash for decrypting the drive if
- you moved the physical drive to another machine
- You forgot your windows password and recovery key

# Full?
When encrypting with bitlocker you choose whether to encrypt 100% of the drive, or to only encrypt the sectors that contain data.