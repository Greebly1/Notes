A hierarchical database of named configuration values that the OS and certain user programs use for settings values.

it is ~15-20mb in size

The registry is constantly getting pounded by read and write requests, so it actually exists on main memory all of the time.
	It is designed for rapid reads and writes

# Keys and Values
The registry is a #key-value database, it is basically a [[Dictionary]] managed by the OS that stores configuration data.
**A key, is similar to a folder**
**A value, is similar to a file**
![[Registry Values]]

# Root Keys
![[Registry Root Key]]

# Registry Hives
![[Registry Hives]]

# Editing the Registry
While you can edit the registry manually using [[RegEdit]]
Most registry edits happen automatically through software.
- It is used to software to communicate, etc
- However even changing settings changes the registry
		Changing display settings
		Anything in the control panel
		etc
