`netsh` is a #Windows  #command utility that allows you to configure and troubleshoot network settings locally or remotely. It can be used for a variety of tasks, including managing software [[Fire Wall]] rules, configuring [[HTTP]] settings, resetting network stacks, and more

It also has functionality to provide the name information as [[netstat]], for instance listing all [[TCP]] connection or [[UDP]] connections

syntax

netsh

opens the net shell

# Some useful commands

netsh interface (ipv4 / ipv6) show interfaces
	gives info on this computer's network adapters

netsh interface (ipv4 / ipv6) show config
	basically an [[ipconfig]]

netsh interface (ipv4 / ipv6) show global
	Shows everything relating to each network adapter and all protocols metadata

netsh int set int name=AsusWiFi admin=disable
	disables or enables an adapter named AsusWiFi
	If it had a space it would need to be in quotes "Asus WiFi"

netsh interface (ipv4 / ipv6) show tcpconnections
	basically a [[netstat]]
	can also do udpconnections


