A #windows-command used to print the name of the computer it is on
Specifically it fetches the computer's [[NetBIOS Name]] , which is stored in the Windows Registry inside [[HKLM]] found at 

HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\ComputerName\ActiveComputerName

# Interesting Considerations
When done inside a windows virtual machine, it will of course retrieve that virtual machine's registry value of the netbios name. Administrators can use branching conditional logic to print the hostnames of certain virtual machines that fit specific criteria, the hostname they get will fall in line with whatever automation tool they used to assign hostnames and they can use it to locate the correct vm.
