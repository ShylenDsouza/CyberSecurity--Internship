Data Breach Awareness & Threat Intelligence Basics

Objective of today's task :

The objective of this task was to understand how cybersecurity analysts investigate data breaches, suspicious IP addresses, and malware indicators using open-source threat intelligence platforms such as HaveIBeenPwned and VirusTotal.

1. Email breach investigation (HaveIBeenPwned)

I used the website https://haveibeenpwned.com/ to check whether an email address appeared in any known data breaches.

What was my observation ?

The email address searched appeared in multiple data breaches (532 breaches). This indicates that the email has been exposed in several publicly known compromised databases.

Data breaches may expose sensitive information such as:

* Email addresses
* Password hashes
* Personal information
* Usernames

Attackers often use this leaked data to perform attacks like credential stuffing, where stolen credentials are used to attempt logins on multiple websites.

Conclusion of the first sub task :

This investigation shows how data breaches can expose personal information and why it is important for users to use strong and unique passwords for different accounts.


2. VirusTotal IP address analysis

VirusTotal is a threat intelligence platform that aggregates results from multiple security vendors to analyze suspicious files, domains, and IP addresses.

IP Address 1: 185.220.101.182

Observation:

VirusTotal shows that 14 out of 94 security vendors flagged this IP address as malicious.

Additional information revealed that:

* The IP is associated with the TOR network infrastructure.
* Community reports indicate SSH brute-force login attempts.
* TOR exit nodes are sometimes used by attackers to hide their real identity.

Conclusion of the sub task :

Because several security vendors flagged this IP address as malicious and it is linked with suspicious activity such as brute-force attacks, it may pose a security risk.

IP Address 2: 103.21.244.0

Observation:

VirusTotal analysis shows:

* 0 out of 94 security vendors flagged the IP as malicious
* The IP address belongs to Cloudflare Inc.
* No suspicious or malicious indicators were detected

Conclusion

This IP address appears to be part of a legitimate network infrastructure and does not show any signs of malicious activity.

3. File hash analysis

The following file hash was analyzed using VirusTotal: 44d88612fea8a8f36de82e1278abb02f

Observation:
VirusTotal results show that:

* 66 out of 68 security engines detected the file as malicious
* The file is identified as the EICAR Test File

The EICAR file is not a real virus but a standardized test file used to verify whether antivirus software can detect potential threats.

Conclusion:

The EICAR file is commonly used by security professionals to test antivirus systems and ensure that malware detection systems are functioning correctly.

4. MY learning outcome:

From this task, I learned how cybersecurity analysts use threat intelligence platforms such as HaveIBeenPwned and VirusTotal to investigate data breaches, suspicious IP addresses, and potentially malicious files.These tools are widely used in Security Operations Centers (SOC) to analyze indicators of compromise and improve overall cybersecurity awareness.
