# 29/01/2018 - 3rd Lecture

## Subnetting

We invested more time to better understand it.

## Drill-down on Ethernet and IP

We understood the difference between Network, Broadcast and Host addresses.

We understood the roles of Ethernet and IP in the realms of LAN and WAN.

We talked about how DHCP, ARP and Default Gateways are all connected.

We used `arp -a` on Windows to see the list of ARP records.

We talked about spoofing ARP responses - allowing an attacker to become the
default gateway for other hosts (also known as MiTM - Man in the Middle).

We talked about using IPv4 fragmentation tricks to bypass firewall.

We used Wireshark to better understand those protocols. We've seen L2 Ethernet
Broadcasts (ARP) and talked about L3 Broadcasts (DHCP).

We understood that the transportation layer (L4) facilitates a communication
channel between processes on (usually) different computing devices (e.g. Client and Server).

## Terms

Sniffer, to Sniff, Encapsulation, Ethernet Frame, IP Packet, UDP Datagram,
TCP Segment, ARP, IP Fragmentation, OSI Model, DoD Model, TCP/IP Model,
Context-Switch (between processes), scheduler (of the operating system),
QoS - Quality of Service, MTU - Maximum Transmission Unit. Access List.

## Homework

1. Read about: DNS, DHCP, TCP, UDP, Firewall, Loopback, PING, ICMP,
Traceroute, TELNET, SSH, TLS, HTTP, NETCAT.

2. Watch Mr. Robot.

3. Practice with https://www.typingclub.com. Reach at least 55WPM.

4. YOU PROMISED :)  Research and public speaking; find at least one
security-related news article and prepare a 2-3 minute talk about it.

5. FINISH IT - WE'LL NEED IT NEXT LESSON: Fill http://bit.ly/2B87gDw with your Twitter, Github, Linkedin.

6. Find the network address and the number of possible different IP addresses for:
    1. 172.3.11.12/1
    2. 1.2.3.4 Mask: 248.0.0.0
    3. 180.1.2.89/29

7. Find the IP and MAC address of your Default Gateway at Home (`ipconfig` / `arp -a`).
Sniff the network and verify that all non-local outgoing ethernet frames
have the SRC MAC Desitnatino of the Default Gateway.

8. Find relevant job descriptions (e.g. SOC Analyst). Put them in Google Docs.
Highlight the different technologies that are required.
