A [[MMC Snap-ins]] utility for managing [[Group Policy]] in [[Active Directory]]
![[GroupPolicyManagement.jpg]]

This utility shows the [[Active Directory]] tree
- It shows all of the [[OU]]s
- It doe snot show specific users though

To use [[Group Policy]], you create a [[GPO]], group policy object; and link it to an [[OU]].
	Now all users part of that [[OU]] will be given the group policy encoded in that [[GPO]]

# Updating Group Policy
Whenever a new GPO is made and linked into an OU, these changes need to be pushed out to users and computers in the domain. This happens automatically every 90 minutes by default or
- You can run the command [[gpupdate]] to manually initiate a group policy update
