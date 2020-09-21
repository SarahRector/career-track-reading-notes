# HTTP: The Protocol Every Web Developer Must Know
https://code.tutsplus.com/tutorials/http-the-protocol-every-web-developer-must-know-part-1--net-31177

* "HyperText Transfer Protocol"
* Is a **stateless** protocol
* *request methods* are sent via URL
  * request uses verbs (GET, POST, PUT, DELETE)
* server responds with status codes and message payloads
* request is sent with URL and verb, server responds with status code and message body

# How DNS Works
https://howdns.works/

* DNS is "domain name system" and it takes the IP address and basicaly gives it a name (google.com, etc)

* the browser and the OS both check their cache to see if they recognize the domain name and if they don't they ask the resolver

* if the resolver (usually your internet service provider) doesn't have it in it's cache it checks with the root server (.com, .org, .net, etc)
  * root servers are scattered all over the globe and are operated by 12 independent organizations
  * each organization also provides access to multiple servers scattered across the globe

* the root server knows how to access the TLD (top-level domain)

* the resolver also caches the information so it doesn't have to ask the root every time

* if the TLD cant find the site, it can find the authoritative name servers for the site, which the resolver can then store for later

* when a domain is purchased, the domain registrar reserves the name and communicates to the TLD registry the authoritative name servers

* the resolver can then run a WHOIS query on the domain and the name server will return the IP address