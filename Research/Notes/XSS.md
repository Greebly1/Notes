Cross Site Scripting

A #Cyber-Attack that exploits [[HTML]] and [[JavaScript]].

Webservers tend to use algorithms and databases to send text data to websites
- comments
- social media posts
- image meta data
- etc

This text is often entered by some person, often not even related to the organization. 
	For instance, a social media user entering a comment, sends that text to a database which will then add it into someone else's [[HTTP]] message so they can read the comment.

If this text contains a <script> </script> tag, and the webserver backend does not properly, it will be interpreted by an end user's client search engine as valid javascript code and execute it.

This is the most dangerous most common #Cyber-Attack 