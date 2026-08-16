# Cybersecurity Incident Report

## Incident Summary

Several customers reported being unable to access the website www.yummyrecipesforme.com. Users received a "destination port unreachable " error message while attempting to load the webpage.

The issue was reproduced by the cybersecurity analyst, who used tcpdump to capture and analyze network traffic.

## Time Incident Occurred

The first DNS request was recorded at: 13:24:32.192571

The first ICMP error response was recorded at 13:24:36.098564


## How the IT Team became Aware

Customers reported that they could not access the company website and received  a "destination port unreachable" error.

the cybersecurity analyst  replicated the issue and began investigation network traffic.


## Investigation Actions

The analyst:

-  Attempted to access the website
-  captured traffic using tcpdump
-  reviewed DNS requests
-  Reviewed ICMP responses
-  Analyzed destination ports and protocols

   ## Key findings

-  Source IP: 192.51.100.15
-  DNS Server : IP: 203.0.113.2
-  Transport Protocol: UDP
-  DNS port : 53
-  Error Protocol : ICMP

Repeated DNS requests for:

Text yummyrecepesforme.com
received the response:

Text UDP port 53 unreachable

the same error occurred multiple times.

##  current status 

The issue remains unresolved and has been escalated to the security engineering team for further invesitgation


## likely cause

The DNS service is not responding on UDP port 53>


Possible causes include: 

-  DNS service unavailable
-  DNS service stopped
-  Firewall rule blocking UDP port 53
-  DNS server misconfiguration

## recommended next steps

-  verify that the DNS server is running
-  Confirm that UDP port 53 is listening
-  Review firewall rules affecting DNs traffic
-  Test DNS resolution after corrective actions
-  Implement DNS monitoring and alerting
-  create a DNS incident response playbook

## lessons learned

A DNS incident response playbook would help standardize future investigation by defining the steps required to validate  DNs services, verify UDP port 53 connectivity, review firewall rules , and  escalate incidents appropriately

This would reduce investigation tie and improve incident rsponse consistency.



