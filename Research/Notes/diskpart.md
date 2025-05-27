A [[Windows]] #command used to manage storage drives

Essentially it is the #TUI for [[Disk Management]]

# Focusing
Before using diskpart you must list and select a disk/drive. 

Some commands automatically change focus

ex

diskpart

list disk

select disk 2

list partition

	ex disk 2 has no partitions
create primary partiton

format fs=ntfs level=backup

# Other uses
Can be used to delete partitions, reformat drives, etc. 