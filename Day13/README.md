Network Traffic Analysis (Wireshark)

Objective:
The objective of this task was to observe real network traffic from my system and understand how data travels across a network using Wireshark.

The Protocol that I Observed :
One protocol observed during the packet capture was DNS (Domain Name System).
DNS is responsible for translating domain names such as `google.com` into IP addresses so that systems can communicate with each other on the internet.

Number of Packets Captured :
Approximately 5300 packets were captured during the packet capture session.

What is my Observation:
One interesting observation was that even when visiting only a few websites, a large number of packets were generated automatically. Many DNS queries and TCP/TLS communications happen in the background between the system and external servers.

Why Packet Capture is Sensitive as per my understanding:
Packet capture is sensitive because it can reveal information such as visited domains, IP addresses, and communication patterns. In some cases, it may also expose sensitive data being transmitted across the network. For this reason, packet capture should only be performed on networks where permission has been granted.
