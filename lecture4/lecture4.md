# 03/02/2018 - 3rd Lecture

## IP Routing

IP Routing protocols - BGP, OSPF, RIP, ISIS, EIGRP.

We understood how LANs and WANs work together.

## UDP / TCP

We understood the difference between UDP and TCP.

We used Wireshark to filter out specific UDP and TCP communications.

(tcp.dstport == 443, udp.dstport == 53).

We understood why UDP is being used by DOS attacks (IP SRC Spoofing), and why
it's harder to achieve such spoofing with TCP.

## DNS Low Level

We studied how recursive DNS resolvers work.

We understood the difference between DNS record types: A, AAAA, CNAME, MX, NS, TXT.

## HTTP and HTTPS

We understood that HTTP is a textual (as opposed to binary) protocol which
uses ASCII to send relevant protocol details such as HTTP Headers / Method / Path.

We understood that HTTPS is (mostly) secure and uses TLS (SSL) which under the hood
employs public key cryptography.

We understood, in high level, how Public Key Crypto works! (proud of you!).

Public keys of servers (google, your bank) come in the form of "certificate".

## Terms
TLD - Top Level Domain, DOS (Denial of Service), ASCII, Hardening, Certificate,
Routing Protocol, PKI - Public Key Infratructure.

## Homework

1. Read about: DNS, DHCP, TCP, UDP, Firewall, Loopback, PING, ICMP,
Traceroute, TELNET, SSH, TLS, HTTP, NETCAT.

2. Watch Mr. Robot.

3. Practice with https://www.typingclub.com. Reach at least 55WPM.

4. YOU PROMISED :)  Research and public speaking; find at least one
security-related news article and prepare a 2-3 minute talk about it.

5. FOLLOW YOUR FELLOW CLASS MATES: http://bit.ly/2B87gDw with your Twitter, Github and Linkedin.

6. Find relevant job descriptions (e.g. SOC Analyst). Put them in Google Docs.
Highlight the different technologies that are required.


7. Use `nslookup` and query different domains for A, AAAA, CNAME, TXT, MX, NS
DNS records. Use Wireshark and save a ".pcap" file with filtered DNS packets
that show queries and answers from servers.
