One of the [[Power Connectors]], made for [[SATA]] hard drives

15 pin connector provides a 12V rail, 5V rail and a 3.3V rail
	the 3.3V rail is rarely used by devices

| Pin | Function                  |
| --- | ------------------------- |
| ~   | L-shaped keying notch     |
| 1   | 3.3V                      |
| 2   | 3.3V                      |
| 3   | Enter/Exit Power Disable  |
| 4   | Ground                    |
| 5   | Ground                    |
| 6   | Ground                    |
| 7   | 5V pre-charge             |
| 8   | 5V                        |
| 9   | 5V                        |
| 10  | Ground                    |
| 11  | Staggered spinup/activity |
| 12  | Ground                    |
| 13  | 12V pre-charge            |
| 14  | 12V                       |
| 15  | 12V                       |

L-shaped key for insertions
	![[SATAPower.jpeg]]

# [[Molex]] to SATA Power
Adapters exist to convert Molex connections into SATA power connectors, in the case a PSU does not have enough SATA connectors
Be warned, these are prone to combustion

Furthermore! These adapters leave out the 3.3V rail, however it is rarely used anyways.
	It won't work for devices that need a 3.3V rail