A #windows-command used to output the contents of the current directory to the user.

# Specials
Dir sort of uses a kind of #Regular-Expression system allowing you to search for specific files in a directory

dir \*.png
	Lists all files in the current directory ending in .png

dir \*.png \*.bat
	Lists all files in the current directory ending in .png or .bat

# Options
**/s** - specified directory
instead of using the current directory, /s allows you to specify a full file path
Additionally it will also specify all sub directories recursively

dir /s "C:\Users\JohnDoe\Documents\DailyReports" \*.pdf 


For further options use 
	dir /?


