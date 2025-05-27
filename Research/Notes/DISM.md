Deployment Image Servicing and Management (DISM.exe) is a [[Windows]] command tool used to manage a windows system image.

Commonly used alongside [[SFC]] to ensure that the cache restore system image is valid.

# Commands

	dism /online /cleanup-image /checkhealth
It just checks if the system image has problems

	dism /online /cleanup-image /scanhealth
A more in depth scan of the system image

	dism /online /cleanup-image /restorehealth
Actually restores the system image

/online
tells DISM to use the current OS image

/cleanup-image

/image:"dir"
Can be used to provide a specific system image for DISM to check against.