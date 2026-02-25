Networking Basics

Objective :
To understand how my system connects to a network and communicates with other systems.

Network interfaces observation (`ip a`):

When I ran the `ip a` command, I observed the following network interfaces:

-> lo (Loopback Interface)  
  This interface is used for internal communication within the system.  
  It has the IP address `127.0.0.1`.

-> eth0 (Ethernet Interface)  
  This is my main network interface that connects my system to the local network and internet.  
  It was assigned a private IP address (192.168.x.x range).

-> docker0 (Virtual Interface)  
  This is a virtual network interface created by Docker for container networking.

From this command, I understood how my system has multiple interfaces for different purposes.

Ping test results:

-> Ping localhost (127.0.0.1)

When I pinged localhost, I received replies with:

- 0% packet loss  
- Very low response time (in milliseconds)

This confirmed that my system’s internal network stack is working properly.

-> Ping google.com

When I pinged google.com:

-> The domain name was resolved to an IP address.
-> I received replies from Google’s server.
-> Response time was shown in milliseconds.
-> Packet statistics were displayed (packets sent, received, loss %).

This confirmed:
-> My internet connection is working.
-> My system can communicate with external servers.

---

What is DNS? :

DNS (Domain Name System) converts human-readable domain names like:

google.com  

into IP addresses like:

142.xxx.xxx.xxx  

Computers communicate using IP addresses, not domain names.  
So DNS acts like the "phonebook of the internet".

Without DNS, we would have to remember IP addresses for every website.



One networking concept that confused me:

I was confused about how DNS decides which IP address to return when a website has multiple servers across different locations.



Conclusion:

From this task, I learned:

-> How to identify network interfaces using `ip a`
-> How to test connectivity using `ping`
-> How DNS resolves domain names using `nslookup`
-> Basic understanding of how systems communicate over networks

This practice helped strengthen my foundational networking knowledge, which is important for my journey in cybersecurity.
