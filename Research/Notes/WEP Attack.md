### 1. 🔁 **IV Reuse**

- IV is only 24 bits → **2²⁴ = ~16 million** possible IVs.
- On a busy network, **IVs start repeating within hours**.
- Repeating IV + same key ⇒ **same RC4 keystream** reused ⇒ vulnerability to keystream recovery.
- If you sniff enough traffick you can repeat an IV and crack the PSK

### 2. 📉 **Weak RC4 Key Scheduling (FMS Attack)**
- RC4's key scheduling algorithm (KSA) is sensitive to certain **"weak IVs"**.
- The **FMS attack** (Fluhrer, Mantin, Shamir, 2001) shows that you can **recover key bytes** by analyzing enough packets with weak IVs.
- Only a few million packets are needed.

### 3. 🔄 **No Replay Protection**
- WEP has no mechanism to prevent [[Replay Attacks]]
- An attacker can resend captured encrypted packets.

### 4. ❌ **CRC-32 Integrity (ICV) is not cryptographic**

- CRC is designed for **error detection**, not security.
- It’s **linear**, so you can **flip bits in ciphertext** and update the CRC accordingly without knowing the key.