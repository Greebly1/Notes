A [[Windows]] #command used to setup the bootable section of the [[Windows System Partition]].
ex

	bcdboot C:\Windows /s S: /f UEFI
Copies the boot system from #c/Windows to the boot sector of the S drive, and specifies that it will use the UEFI version.

# Installing Windows
bcdboot will not partition and format a drive, however it does everything else needed for installing a bootable version of windows

If you combine bcdboot with [[diskpart]], you can create a full windows installation just through the command line.