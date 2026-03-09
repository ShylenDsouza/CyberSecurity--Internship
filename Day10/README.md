Firewall Basics

Objective:

The objective of this task was to understand how a firewall works and how to check firewall status and create a basic rule using UFW (Uncomplicated Firewall) in Linux.

Firewall Status Check:

First, I checked the firewall status using the command:

sudo ufw status

The output showed that the firewall was already active and some rules were already configured.

Firewall Rule Created:

I created a firewall rule to allow SSH traffic through port 22 using the following command:

sudo ufw allow 22

After executing the command, the system confirmed that the rule was successfully added.

Verification of the Rule:

To verify the rule, I ran the following command again:

sudo ufw status

The output showed the rule:

22/tcp ALLOW Anywhere

This confirms that traffic on port 22 is now allowed by the firewall.

Difference Before and After:

Before creating the rule:
The firewall was already active but the new rule allowing port 22 had not yet been added.

After creating the rule:
The firewall rule allowing port 22 appeared in the firewall status list, meaning SSH traffic is permitted through the firewall.

Why Firewall Alone Is Not Enough

A firewall only controls which network traffic is allowed or blocked. It does not protect the system from malware, phishing attacks, weak passwords, or software vulnerabilities. Therefore, other security measures such as regular system updates, strong passwords, monitoring tools, and antivirus software are also required for complete protection.

New Concept Learned:

In this task, I learned how a firewall uses rules to control network traffic. By allowing or blocking specific ports, we can manage which services are accessible from outside the system.
