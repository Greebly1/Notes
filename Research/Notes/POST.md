Power On Self Test

When a computer turns on, the first thing the [[UEFI]]/[[BIOS]] [[Firmware]] does is perform a POST.

Every device on the motherboard, as well as every interface is given a special command/signal to perform a POST.

Each device will check itself for power issues, for instance a NIC will check if any of its power pins are giving a strange voltage output, indicating a short or power failure.

The result of these individual POSTs are communicated back to the CPU. 


![[POST Beep Codes]]

![[POST Card]]