Also called the Front Side Bus (FSB)

The system bus tends to be a #Legacy parallel communication bus that older CPUs used.

# Components
The FSB was a combined bus of
- Data Bus
- Address Bus
- RW Line
- Optionally, [[IRQ Line]]s

If a device is connected to the FSB, that means at some level the CPU communicates to it through memory address reads and writes. 

# [[North Bridge]]
The system bus or FSB was a set of pins from the CPU itself. 
- Address Pins
- Data Pins
- R/W Pin
- Interrupt Pin(s)

Instead of being directly connected to devices such as GPUs, RAM, etc, the FSB passed through an external chip called the North Bridge. 