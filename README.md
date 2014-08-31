Router is the documentation for my custom net device.  I am using it to provide a number of services on my lan.

- wifi to ethernet router (nat)
- development http server
- git server
- development sql server
- provide local network convinece services
  - dhcp server
  - netbios nameserver
  - local dynamic dns server
- act as a file server using nfs and cifs

Included in this project are several config files and convinence scripts

**Configuration Files**
- **smb.conf** the base configuration for smbd, includes the cifs file sharing and netbios services
- **dnsmasq.conf** Dnsmasq's provides dhcp server and local dns services

**Convinence Scripts**
- **ifreset** calls ifdown then if reset for the specified device
- **iftest** returns the class c network the host is on
- **ip-nat** a script for the debian init system it sets the routing tables for ip masquerading

