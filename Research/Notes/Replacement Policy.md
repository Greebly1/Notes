
What algorithm a cache system uses when replacing old cache with new data from RAM.

Wikipedia: https://en.wikipedia.org/wiki/Cache_replacement_policies

A good replacement policy will not replace data that is constantly constantly used. Important data such as kernel scheduling data would perpetually remain in cache for fast access. 
However, the replacement policy should also remove data that doesn't even get accessed, to make room for better more useful data.