Network Scanning Basics (Nmap)

1. Open ports observed
After performing a basic scan using:

nmap 127.0.0.1

No open ports were detected on the system. All scanned ports were in closed state.

2. Service detection result

Using the command:

nmap -sV 127.0.0.1

Nmap attempted to detect services and versions running on the system. Since there were no open ports, no services were identified.


3. Fast scan result

Using the command:

nmap -F 127.0.0.1

The fast scan checked the 100 most common ports. All ports were closed on the localhost system.

4. Why open ports can increase security risks?

Open ports indicate that services are running on a system. If these services contain vulnerabilities or are misconfigured, attackers can exploit them to gain unauthorized access to the system.

Therefore, security professionals regularly scan systems to identify open ports and reduce the attack surface.

5. The new concept that I learnt 

In this task, I learned how Nmap performs port scanning to identify open ports and running services. I also learned the difference between a basic scan, service detection scan, and fast scan.
