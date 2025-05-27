A #Windows OS stability feature that allows the system to save [[Restore Points]] and return to those points in the case of future instability.

A restore point stores all relevant system configuration and back up data. So in theory loading a restore point and overwriting the current configurations and systems will put the system to a past state where things were stable.

# Automatic Restore Points
Restore points are made automatically when certain events occur.
- Before downloading a program
- Just before an OS update
- Weekly or monthly (configurable)
- When a restore point is loaded by user (Creates an undo restore point)

# Password And Cryptographic Keys
Very important authentication data such as passwords and cryptographic keys should be backed up before loading a restore point.

If you have changed your password it is a good idea to make a [[Password Reset Disk]]