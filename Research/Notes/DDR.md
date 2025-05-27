Double Data Rate
A [[RAM]] bus technology that allows data to be read back on both the rising and falling edge of a clock cycle. Of course this means it must be [[SDRAM]] 

Effectively this doubles the data throughput, although it is mostly used for caching nearby data.

1. The CPU will request a value at a memory address ex (mov RAX 0x1000)
2. The memory controller decodes it into column, row and bank addresses
3. The memory controller strobes the correct lines on the DDR RAM bus.
4. At the rising edge of the next clock cycle, the value is returned to the CPU
5. At the falling edge of the cycle another value, usually the next value is sent to the CPU and cached 
# ![[System Memory Form Factors]]
  # ![[DDR Versions]]