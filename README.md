# ldap_mail
A simple &amp; safe mail server skeleton around LDAP

### What is this?
* A personal project to create a fullblown self-hosted mail server with LDAP backend.
* Easy on resources
* Using only free, open source and battle tested solutions
* Safe & modern implementing SPF, DKIM and DMARC for both inbound / outbound
* Very restrictive access: tcp/25 only from inbound, tcp/465 (ssl/tls) + tcp/587 (starttls) only authenticated SMTP/S, tcp/993 (ssl/tls) IMAP/S

### What this isn't
* A sinlge command turn-key solution
* A microsoft flavored fancy gui bloatware

### Created from scratch. Kinda.
It was indeed created from scratch because no other solution fit my needs. Despite other projects being much more mature with a nice admin interface and very close / being properly turn-key, like Mailu or Mailcow etc. they just couldn't be tailored to do what I wanted to achieve without serious overriding. At which point I decided I might as well dig deep. 

### Credits
* Mailu: Altough this isn't a straight fork it was heavily influenced with some straight reused and inspired configuration codes from Mailu

### Prerequisites
* a linux host with the Docker daemon and docker-compose
* an existing LDAP backend configured with your domain, preferably FreeIPA (for example https://hub.docker.com/r/freeipa/freeipa-server/)
* an existing SSL certificate, preferably wildcard (get one from letsencrypt!) 
* .. plus the usual (tcp/25 accessibility, an fqdn etc.)



