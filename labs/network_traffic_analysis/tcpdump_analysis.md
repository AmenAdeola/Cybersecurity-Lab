# Tcpdumo analysis


## DNS Request

Source:
192.51.100.15

Destination:
203.0.113.2

Protocol:
UDP

Port: 
53

Query:
A? yummyrecipesforme.com

##Error Observed

ICMP:
udp port 53 unreachable

## Interpretation

The DNS resolution process failed before the HTTPS request could be sent to the website server
