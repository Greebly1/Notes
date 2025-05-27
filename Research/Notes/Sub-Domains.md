A sub-domain is a part of a larger domain.

Many organizations operate their own [[Authoritative Name Server]] that hosts their domain
	They can actually create more subdomains off of this domain

blog.example.com
en.example.com
fr.example.com

The DNS system will query for this subdomain in the example.com authoritative name server, which might know the IP or it might know where to ask.
	The French Wikipedia servers might be located in France, thus they would have a different IP form the Russian Wikipedia servers.

