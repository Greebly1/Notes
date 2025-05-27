#windows-command  used to copy files from command line. One of a few [[Windows Copy Commands]].
aka - eXtended copy

syntax

xcopy "source path" "destination path" options

# Important Options
/E - copy all subdirectories including empty ones
/H - copy hidden files and system files
/C - continue even if an error occurs (ex, NTFS file permissions)
/I - assume the destination is a folder even if it doesn't exist
