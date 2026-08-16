# Networking DoS attacks cheat sheet

| Attack Type | Protocol | How it works | Impact |  
|-------------|----------|--------------|--------|
|Ping Flood | ICMP | sends a large number of ICMP Echo Requests (Ping Packets| Network congestion and resource exhaustion|
|SYN Flood| TCP | Sends many SYN packets but never completes the TCP handshake| Server resources become exhausted and legitimate connections are blocked|
|UDP flood| UDP | Sends a large volume of UDP packets to random ports| High network traffic and system resource consomption|
|DNS Flood| DNS/UDP| Sends massive numbers of DNS requests to overwhelm a DNS server| DNS server become unavailable and website cannot be resolved|
|HTTP flood| HTTP/HTTPS | Sends excessive web requests to a web server| Website slowdown or outage|
|DNS Amplification | DNS | Uses small spoofed requests that generate much larger DNS responses | Amplifies traffic and overwhelms the victim|
|Smurf Attack | ICMP | Sends ICMP requests to broadcast addresses causing many systems to responds A network attack performed when an attacker sniffs an authorized user’s IP address and floods it with ICMP packets| Large spikes of network traffic overwhelm the victim|




# DoS attacks to remember 

| Attacks type | Remember |
|--------------|----------|
| Ping flood | Too many pings|
| SYN Flood | Half-open TCP connections|
|UDP Flood | Too many UDP packets |
| DNS Flood | Too many DNS requests |
| HTTP Flood | Too many website requests |
| DNS Amplification | Small request -> huge response|
| Smurf attack | Many ICMP replies at once|
