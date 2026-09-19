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
sudo tcpdump -w capture.pcap |Save packets to a PCAP file| Sudo tcpdump -w capture.pcap
sudo tcpdump -i eth0 -nn -c9 port 80 -w capture.pcap| Capture HTTP traffic and save to file|sudo tcpdump -i eth0 -nn -c9 port 80 -w capture.pcap
ls -l capture.pcap|Verify capture file exists| ls -l capture.pcap|

# Read PCAP Files

Command|Purpose|Example|
-------|-------|-------|
sudo tcpdump -r capture.pcap | Read packets from pcap fiel|sudo tcpdump -r capture.pcap
sudo tcpdump -nn -r capture.pcap -v | Read detailed packet information| sudo tcpdump -nn -r capture.pcap -v
sudo tcpdump -nn -r capture.pcap -x| Display packet contents in hexadecimal and ASCII| udo tcpdump -nn -r capture.pcap -x


# Tcpdump Options Learned

Option|Purpose|
------|-------|
-i| Specify network interface
-D | List capture interfaces
-v | Verbose output
-c | Capture a specific number of packets
-nn | Disable hostname and port resolution
-w | Write packets to a file
-r | Read from a capture file
-x | Display hexadecimal and ASCII output
& | Run command in the background


# Traffic Generation Commands

Command|Purpose|Example|
-------|-------|-------|
curl| Generate HTTP traffic| curl
curl https://example.com|Retrieve website content | curl https://example.com


# Common Packet Fields

Field | Meaning|
------|--------|
Source IP| Sending host
Destination IP | Receiving host
TTL | Time To Live
Port | Network service used
Flags| TCP Packet behaviour
Length | Packet size in bytes
Protocol | Communication protocol


# Frequently Seen TCP Flags

Flag | Meaning|
-----|--------|
S| SYN
A|ACK
F|FIN
R|RST
P|PUSH

