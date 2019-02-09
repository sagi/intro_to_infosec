# 06/02/2018 - 5th Lecture

## NAT

We understood how NAT (Network Address Translation) and PAT
(Port Address Translation) are used by Routers to translate between
local, usually unrouteable IP addresses (e.g. 10.0.0.1), and a public,
routable IP address.


## DHCP

DHCP (Dynamic Host Configuration Protocol) drill down. We understood how it
works. DHCP Discover, DHCP Offer, DHCP Request, DHCP Ack, DHCP Nack.


## ICMP, PING, TRACEROUTE

We understood how `ping` works and that it's used to measure the RTT -
round trip time - between two endpoints.

We understood how the speed-of-light is useful in calculating the lower bound
of a communication link RTT.

We understood how we can use the TTL field in a IPv4 header to gain more info
on the routers the packet

We understood how traceroute (tracert) uses ICMP Ping Echo requests with
different TTLs,


## Netcat

We used `netcat -k -l 1234`, to open a TCP server on port 1234, and then
used the chrome browser with the url: "http://127.0.0.1:1234/" and saw
the text of the HTTP1/1 GET request.


## Common Protocol Ports

- tcp/80 - HTTP
- tcp/443 - HTTPS
- tcp/23 - TELNET
- tcp/22 - SSH
- tcp/21 - FTP
- tcp/25 - SMTP
- udp/53 - DNS
- udp/666 - DOOM
- udp/68 - DHCP Client
- udp/67 - DHCP Server


## HTTP

We've seen how an HTTP header looks like:

```
GET /100269.jpg HTTP/1.1
Host: yshops-ads.ynet.co.il
Connection: keep-alive
Pragma: no-cache
Cache-Control: no-cache
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36
Accept: image/webp,image/apng,image/*,*/*;q=0.8
Referer: https://z.ynet.co.il/mShort/commerce/2018/YnetShopsIframe
Accept-Encoding: gzip, deflate, br
Accept-Language: en-IL,en;q=0.9,he-IL;q=0.8,he;q=0.7,en-US;q=0.6
```

HTTP Methods: GET, POST, PUT, DELETE, HEAD, OPTIONS - we'll survey them
next lesson (probably).


## Windows commands

- `ipconfig /all`
- `ipconfig /release`
- `ipconfig /renew`
- `arp -a`
- `arp -d *`
- `tracert -d 4.2.2.2`


## Linux commands

- `ifconfig`
- `ip addr`
- `tracepath -n 4.2.2.2`


## Terms

RTT - Round Trip Time, "Ledabeg" - to debug, Infoleak - information leakage,
Online presence, Port, "Lefarser" - to parse.


## Homework

1. Read about: HTTP, HTML, CSS, Javascript, API

2. Watch Mr. Robot.

3. Practice with https://www.typingclub.com. Reach at least 55WPM.

4. Research and public speaking; find a topic - either a technologoy (e.g. DNS, DHCP)
or a security-related news article and prepare a 2-3 minute talk about it.

5. FOLLOW YOUR FELLOW CLASS MATES: http://bit.ly/2B87gDw with your Twitter, Github and Linkedin.

6. Find relevant job descriptions (e.g. SOC Analyst). Put them in Google Docs.
Highlight the different technologies that are required.

7. Use `netcat`, create a TCP server on port 1234. Use chrome and open
http://127.0.0.1:1234/. Capture everything with Wireshark and save a ".pcap"
file. Make a screenshot of the HTTP request in `netcat` and show me next
lesson! :)


<hr>
Copyright 2019 Sagi Kedmi
