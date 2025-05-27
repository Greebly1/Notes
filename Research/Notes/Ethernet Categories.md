Tags: #Hardware [[Ethernet]] [[PHY Rate]]

Not all copper is made equal, we have many different categories (abbreviated as *cat n*), different cable sheaths, coatings, and shapes with specific use cases.

# Governing Body
The Ethernet cabling standards are made by the Telecommunications Industry Association #TIA.

# Categories
Cables are broken into categories based on frequency, shielding, length, copper core type, and number of wires.
Today we only really operate with cat 5 and above.
Note: The max lengths of most categories can only be achieved with solid core cables see also [[Solid vs Stranded Core]]

|            | [[PHY RATE]] | Length       | Additional Info              | Encoding            | Freq   |
| ---------- | ------------ | ------------ | ---------------------------- | ------------------- | ------ |
| **Cat1**   | 1 Mb/s       |              | Telephone wire, 2 wires      | Analog voice        | 400KHz |
| **Cat2**   | 4 Mb/s       |              | IBM Token Ring, 2 wires      | Analog voice        | 4MHz   |
| **Cat3**   | 10 Mb/s      | 100 m        | 10GBaseT, token ring         | Manchester          | 16MHz  |
| **Cat4**   | 16 Mb/s      | 100 m        | IBM Token Ring               | Manchester          | 20MHz  |
| **Cat5**   | 100 Mb/s     | 100 m        | 100GBaseT                    | 4B/5B + MLT-3       | 100MHz |
| **Cat5e**  | 1 Gb/s       | 100 m        | Residential gigabit ethernet | 4D-PAM5             | 100MHz |
| **Cat6**   | ~10 Gb/s     | 50 m         | 1 Gb/s after 50m, commercial | 4D-PAM5             | 250MHz |
| **Cat6a**  | 10 Gb/s      | 100 m        | Data centers and commercial  | DSQ128 (over PAM16) | 500MHz |
|            | **     Non** | **Official** | **Proprietary Categories**   |                     |        |
| **Cat7**   | 10 Gb/s      | 100 m        | Does not fall off            | DSQ128 (over PAM16) | 600MHz |
| **Cat7a**  | 40 Gb/s      | 50 m         | 10 Gb/s after 50m            | PAM4                | 1GHz   |
| **Cat8.1** | 25 Gb/s      | 30 m         |                              | PAM4                | 2GHz   |
| **Cat8.2** | 40 Gb/2      | 30 m         | cutting edge data center     | PAM4                | 2GHz   |

A cable's PHY Rate is mainly based on two factors.
- The protocol/encoding scheme used
- The max frequency
Going above a cable's max frequency will cause data loss due to crosstalk between the wires and reflections through the other end. Higher rated cables typically are twisted more tightly to reduce crosstalk and increase frequency. 
	The number of twists per inch or meter is called its twist rate or pitch ~5 per inch for cat5

