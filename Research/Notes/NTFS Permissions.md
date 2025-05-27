A permission is a specific control given to a [[Windows Account]] or [[Windows Group]] in [[NTFS]] over a file or directory

**Permissions**
- List Folder Contents
- Read
- Read & Execute
- Write
- Modify (write and delete permission)
- Full Control

# Inheritance
Permissions are either 
Explicit (black checkmarks)
	Assigned to that folder with intent
Inherited (gray checkmarks)
	Interpreted based on a parent folder's permissions (which themselves may be inherited as well)

![[NTFSInheritedPermissions.png]]

# Advanced Permissions
Even more fine grain control can be given
But this is too damn specific form e to care
#TODO 14 advanced permissions