# elevate-labs-cybersec-task-4-or-Basic-Firewall-Management-Exercise
# Basic Firewall Management Exercise



# Objective

To gain hands-on skills in managing firewall rules (Allow/Deny), testing network connectivity, and understanding the core principle of network traffic filtering.

# Environment

This guide provides steps for two common environments:

* Linux: Using UFW (Uncomplicated Firewall) via the terminal.
* Windows: Using Windows Defender Firewall via the Command Line (`netsh`) or GUI.


# Exercise Steps & Documentation

The following steps were executed to demonstrate firewall functionality:



1.Search for "Windows Defender Firewall with Advanced Security".
2. Select Inbound Rules in the left pane to view the list.
3.
1) Right-click Inbound Rules New Rule... 

2) Rule Type: Port  Next 

3) Protocol: TCP Specific local ports: 23 Next 

4) Action: Block the connection  Next 

5) Profile: Check all three (Domain, Private, Public) Next \

6) Name: TEST_BLOCK_TELNET_23  Finish

4) Test Rule Test with telnet as described above.
5) Remove Block Rule Find the rule TEST_BLOCK_TELNET_23 in Inbound Rules, right-click, and select Delete.

#Key Outcome: Traffic Filtering Summary

A firewall filters network traffic based on an ordered set of rules by inspecting the Source/Destination IP, Protocol (TCP/UDP), and Port Number.

* ALLOW (Accept): Traffic matching the rule is permitted.
* DENY (Reject/Block): Traffic matching the rule is stopped.
* Implicit Deny: Any traffic that does not explicitly match an **ALLOW** rule is automatically blocked. This is the core security principle.
