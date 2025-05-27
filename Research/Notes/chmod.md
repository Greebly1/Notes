A #Linux #command used to change the permissions of a file.

  # ![[Linux File Permissions]]
# Command
chmod (3 digit number) /directory/example.png

Each digit determines a different user permission
First digit
	Owner
Second digit
	Group
Third digit
	Others
![[CHMODCheatsheet.png]]

So for example
	chmod 755

Only gives the owner access to change the file, but allows the rest of the owners group and any other users to read and execute any files.

# Options

**-R**
Recursive, will apply this command to every file within a directory, if the target is a directory
	chmod -R 777 /example/

**-V**
Verbose, will log each command output to the terminal as the command is executed.
	chmod -V 777 /example.png

**-F**
Forced, will continue with the command even if errors occur. Instead of halting it will just continue
	chmod -F -R  777 /multiUserDirectory/

# Symbolic Mode
The permissions can be represented as symbols
R-Read
W-Write
X-eXecute

These are the same symbols visible when you use [[LS]]

chmod -R -F rwxr-xr-x /example/

Furthermore the different users have their own symbols
	U-Owner
	G-Group
	O-Other
	A-All
	UGO-All

When using chmod with the user symbols, simply subtract (-) or add (+) permissions.
Also you can = if you want to set the permissions to the symbols exactly

So chmod can be used like
	chmod o-x /example.py
	chmod og+w /example.py
	chmod ugo=rwx /example.py