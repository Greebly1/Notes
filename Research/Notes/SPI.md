Serial Peripheral Interface
A data bus standard used for devices and printed circuit boards to communicate.
It uses 4 wires, and is #full-duplex.

# Master-Slave Topology
SPI uses a master-slave topology, whereby a master node controls control signals to slave nodes.
It is however typically full duplex.

The master node will use a select wire to select which slave node to read/write

Each clock cycle of the clock wire, both the master and the selected slave will send 1 bit on their lane. 

Word sizes differ by device, from 8-16 bit word sizes.

# Uses
Typically used by embedded devices such as, [[TPM]], Real Time Clocks, Touch-Screens, digital-to-analog converters, temperature readers, etc.

# Pros
SPI actually has a higher data throughput than [[I2C]].
