Tags: [[Ethernet]]

Some ethernet capable devices support a special feature named Power Over Ethernet (POE). It is convenient for devices located far from power outlets; security cameras, smart home controllers, and ceiling-mounted wireless access points. 
	The convenience comes from only needing to run 1 cable.

# How
Due to the encoding system that Gigabit Ethernet uses (also Cat5e) (also 1000GBaseT), signals are interpreted as relative values compared against a voltage floor.
If say, a flat 5 volts are added to the signal, then the voltage floor will be 5 volts above ground.
This allows the device to siphon out that extra 5 volts to power itself.
	Note: Due to the extra voltage, the cables do heat up more. It is recommended to use POE improved ethernet cabling and solid core.
# POE Injector
![[POEInjector.webp]]

# POE Switch
Best used when several POE devices must be supported
![[POESwitch.webp]]