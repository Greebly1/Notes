Pre-Shared Key

A #Cryptography key derived from a network password which is manually entered in, intended to provide #authentication to a device.

It is usually 128 bits long, but varies in length depending on implementation

Usually it is computed with
- The [[Wifi Password]]
- The [[SSID]]
- Many iterations of [[HMAC-SHA1]]

The PSK will be the same for all devices in the network