#Temporal-Key-Integrity-Protocol
A temporary stopgap security mechanism to replace [[WEP]]'s severe flaws for use in [[WPA]]

It is mostly built on WEP, at the time it was mostly a firmware patch that attempted to improve it.

# IV Size
Instead of a 24 bit IV, TKIP uses a 48 bit IV, this way it repeats IVs much much MUUUCH rarer.

# Key Mixing
Instead of just prepending a [[IV]] to a #PSK, TKIP combined the two.
	Instead of cutting the deck they shuffled it. This makes it much harder to extract the PSK if an attacker gains access to it.

# Replay Protection
TKIP includes an incrementing sequence counter that can be used to stop [[Replay Attacks]]

# Message Integrity
TKIP contains a 64 bit [[Michael MIC]], which includes a 32 bit CRC. MIC protects against man in the middle attacks and data corruption detection.

# Security Flaws
TKIP was just a bandaid, it still contained fundamental flaws that have been exploited
1. A flaw in the Michael MIC protocol allows attackers to guess a MIC value after about 12 minutes
2. The [[NOMORE]] attack