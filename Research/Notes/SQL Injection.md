A #Cyber-Attack that leverages [[SQL]] to target a database.

Unlike other code injection attacks, this one targets the backend.

Over time after the internet was created, developers realized that a website made for multiple users, really is, at an implementation level, just a database that serves HTML to different users.
This means that in site searchbars, such as a youtube search bar sends a SQL message to a database derived from what the user entered.
	Now if the user entered a SQL escape sequence, then the SQL parser would interpret the next lines as commands.
Now you can execute anything on the server, such as find and change passwords, or delete the entire database.