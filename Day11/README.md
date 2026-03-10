Network Services (TryHackMe)

Objective:

The objective of this task was to understand what network services are and how they communicate using ports in a network environment.

Network services are applications or processes that run on a system and listen on specific port numbers. These services allow systems to communicate with each other over a network.

Example Network Service

SSH – Port 22

SSH (Secure Shell) is a network protocol that allows secure remote login and command execution on another system. It encrypts the communication between the client and server, making it safer than older protocols like Telnet.

Connection to Port Scanning:

In Day 9 we learned how to use Nmap to discover open ports on a target system.

Example command:

nmap <target-ip>

If port 22 is open, it usually means that the SSH service is running on the target machine.

Port scanning helps security professionals identify services running on a system and detect potential vulnerabilities.

Connection to Firewall:

A firewall controls incoming and outgoing network traffic based on predefined security rules.

For example:

-> A firewall can allow SSH access only from trusted IP addresses
-> It can block port 22 from external networks

This helps prevent unauthorized access and improves system security.

Concept that I learnt :

After completing the TryHackMe Network Services room, I learned that open ports usually indicate active network services. Attackers often scan systems to identify these services and exploit vulnerabilities. Understanding services and ports helps cybersecurity professionals secure systems and reduce the attack surface.
