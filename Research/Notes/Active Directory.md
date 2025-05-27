An #Enterprise user management system that runs on a [[Domain Controller]]. 

It manages a [[Windows Domain]]

Essentially a database for user account information, privileges and policies.


# How it works
When a user logs in, Active Directory authenticates their credentials (username and password)
- based on their assigned rights, they are given access to certain organization resources as well as be restricted from certain features through a security policy
		This is done through [[Group Policy]]

To manage active directory, you must either be logged onto the domain controller, or logged into a domain-connected admin account on a machine with [[RSAT]].
- Open the [[Active Directory Users and Computers]] utility

For security and authentication, Active Directory uses the [[Kerberos]] protocol.

# How to Set Up a Domain
1. With a windows server machine, create a domain through the active directory domain service. Create a domain name, document this name.
2. Configure a [[NetBIOS]] name derived from the domain name
3. Create a user and add them to an admin group, give them an admin password, document this username and password
4. Use IPConfig to find the Domain Controller's IP. Make sure it is set up using a static IP
5. Open another windows machine (non Home edition) connected to the LAN.
6. Change its primary DNS server to point to the Domain Controller
7. Change the secondary DNS server to be some default fallback, such as 8.8.8.8
8. In System Properties, change the computer from a workgroup to a domain
9. Enter domain name. 
10. Enter the admin credentials
11. This machine is now part of the domain, and will appear in active directory

# Domain Trusts
![[Domain Trusts]]