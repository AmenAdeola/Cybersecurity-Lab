# Networking Monitoring Commands

Command|Purpose|Example|
-------|-------|-------|
ifconfig| Display network interface configuration|ifcongig
tcpdump|Capture and analyze network traffic| sudo tcpdump
tcpdump -D| List available capture interfaces|sudo tcpdump -D
curl| Generate web traffic or retrieve web content| curl opensource.google.com

# Tcpdump Commands

Command|Purpose|Example|
-------|-------|-------|
sudo tcpdump| start packet capture| sudo tcpdump
sudo tcpdump -i eth0| Capture traffic on a specific interface| sudo tcpdump -i eth0
sudo tcpdump -i eth0 -v | Display verbose packet information| sudo tcpdump -i eth0 -v 
sudo tcpdump -c 5 | Capture only 5 packets| sudo tcpdump -c 5
sudo tcpdump -i eth0 -v -c5| Capture 5 packets with detailed outup| sudo tcpdump -i eth0 -v -c5
sudo tcpdump -nn|Disbale hostname and port resolution| sudo tcpdump -nn
sudo tcpdump port 80| Filter HTTP traffic| sudo tcpdump port 80
sudo tcpdump host 172.17.0.2| Capture traffic involving a specific host| sudo tcpdump host 172.17.0.2

# Packet Capture File Commands

Command|Purpose|Example|
-------|-------|-------|

# Read PCAP Files

Command|Purpose|Example|
-------|-------|-------|

# Tcpdump Options Learned

Option|Purpose|
------|-------|

# Traffic Generation Commands

Command|Purpose|Example|
-------|-------|-------|

# Common Packet Fields

Field | Meaning|
------|--------|

# Frequently Seen TCP Flags

Flag | Meaning|
-----|--------|


