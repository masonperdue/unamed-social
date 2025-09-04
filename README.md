# unamed-social
Unamed Distributed Opt-In Social Media Platform Using Open Standards and Tools

* DOISP - the Distributed Opt-In Social Platform (Not Available)
* JSON files 
* inspired by rss/atom feeds
* uses open formats and protocols 
* server is http(s) site the hosts an index.json and posts.json as well as media 
* each post is named with publication date
* posts are removed one year (?) after publication - checked every time a post is made by client
* server must also have a file server (samba, ssh, SFTP?) to allow authenticated clients to add/remove files and update the index
* server is entirely passive - all work is done by the clients
* write the clients in bash and a setup script for the server using (Apache/caddy and samba?) 
* use gnupg and sha256 to hash, encrypt and sign uploads/downloads (if the server has an active rule) or not (use secure file sharing only) 
* look at PUT/POST/GET commands - only http?
* use base64 "password" to hide URL or root directory for https(s) server or for each user and only allow them access to their directory to create "privacy"
* each post should be a json file with date, title, poster, server, media, text (include special characters for location of media like \img0 \vid1 \aud1)
* client application in bash using curl to pull most recent posts and list dates and titles to choose which to display (add media insertion later)
* make Android, windows, Linux, iOS apps after website
* test first on LAN then host with ip on wan then buy domain name
* figure out if possible to securely upload files after authenticating through https? with curl?
* Use Apache HTTPD and Basic HTTP Authentication to limit PUT, POST, DELETE while allowing GET for all - add encryption for HTTPS later
