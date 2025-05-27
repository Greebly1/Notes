[[WiFi]]

Wired Equivalent Privacy (WEP)

For years this was the 'security' that was used with wireless connections. It was made for 802.11a and 802.11b [[WiFi Standards]].

# Security Vulnerability
In 2001 a critical security vulnerability was discovered in the core protocol.
Several amendments to the protocol were made, WEP2, up to WEP104
	Due to hardware constraints, devices using WEP could not be replaced easily, only firmware updates could attempt to solve the issue.
# Deprecation
All forms of WEP were not secure, due to certain static unchanging elements of the protocol going forward. IEEE officially deprecated the protocol in 2004, replacing it with [[WPA]]

New devices that use 802.11a and 802.11b for backwards compatibility will do so with WPA instead of WEP.
	For security reasons it is recommended to not even allow wireless devices to communicate with older WEP-only devices. This is often the case

# How it works
WEP is based on the [[RC4 Stream Cipher]] to generate a [[Keystream]]
1.
All clients share the same [[PSK]], either a 40 bit one or a 104 bit one
	WPA64 --> 40 bit PSK
	WPA128 --> 104 bit PSK

2.
Generate a 24 bit [[IV]]

3.
Prepend the IV to the PSK, now we either have 64 bits of key seed or 128 bits

4.
Use it to generate a RC4 Key stream

5.
All of the data alongside a 32 bit [[CRC]] is [[XOR]]'d with the keystream

6.
The IV is sent in plaintext along with the encrypted message


![[WEP Attack]]