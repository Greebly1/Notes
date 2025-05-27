#Linux #command utility for installing and managing packages and dependencies

# How it Works
yum checks a database repository which contains all Linux packages.

yum install packageName
	will ask you y/n

yum remove packageName

yum erase packageName

yum clean
	removes any dependencies leftover from a deleted package

yum list
	lists all packages

yum list available
	lists all packages that are available

yum list install
	lists all installed packages

yum update packageName

yum upgrade packageName

yum search packageName
