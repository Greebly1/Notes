System File Checker, a #Windows system stability and restore feature.

The windows operating system is a myriad of critical system files. System instability occurs when one of these system files gets deleted, moved, corrupted, renamed, etc.

# System Image
SFC has a (hopefully uncorrupted and up to date) system image it uses to check if system files are corrupted or not.

If it finds mistakes in files, it fixes them.

It can even clean up a DLL Injected [[Phage Virus]] as long as the system image has not been corrupted by the same malware.

# System Image Coherency
The system image may not be up to date, portions of it may date back years, and it itself may be corrupted.

If this is the case, and it likely is, you should utilize [[DISM]]

# SFC Commands
From within an administrator console, run

	sfc /scannow

This will run the system file checker and repair corrupted files.

/OFFLOGFILE
a flag that tells the scan to dump the offline log files to the console during the scan.