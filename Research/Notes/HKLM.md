HKEY_LOCAL_MACHINE
The most important [[Registry Root Key]]

Stores config data about the settings for this machine

Contains several important Subkeys
- [[SAM]] 
- Security (only accessible by admin)
- Software (config data for non-portable software)
- Hardware (generated during boot, not saved to disk)
- Components
- [[BCD]].dat

When saved as a hive, HKLM is broken into each of its subkeys and saved to different areas on disk
- BCD goes to #systemreserve/Boot
- The rest go to #c/Windows/system32/config