[[Group Policy]] Object

A single unit of group policy, however only one group policy is needed to edit **all** user settings.
- It is good practice to separate specific policies into different, smaller GPOs easier to individually manage

The [[Group Policy Management]] utility allows you to configure your GPOs for different settings such as a logon script, security, user access control, etc.

From a low level, all a GPO does is provide a streamlined way of editing the [[Windows Registry]] for domain accounts.
	All of these features are available in the registry already, they just suck to use that way.

# Linking
To apply GPOs, you link them to an [[OU]]. Furthermore, you can filter what [[Security Group]]s the GPO applies to.