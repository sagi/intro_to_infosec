# 20/02/2018 - 9th Lecture

## Test #1 Review

We solved Test #1 together.

## Sprunge

We installed an alias for `sprunge` and added it to our `~/.bashrc`.

## DAC, MAC, Whitelist and Blacklist

We explained DAC and MAC again, and how strategies such as Whitelist or
Blacklist help us.

## We Reviewed a Vulnerability Research Blogpost Together

The research: [https://www.mauritsvanaltvorst.com/rce-chinese-ip-cameras/](https://www.mauritsvanaltvorst.com/rce-chinese-ip-cameras/).

Through reviewing the article we learned how vulnerability research is done
within a LAN.

We explained why and in what setup the researcher used `nmap`.

We explained how and why the researcher injected payloads such as `$(sleep 5)`
and `$(ping <his LAN IP Address>)`, easily achieving RCE (Remote Code Execution).

We then saw how the researcher used the contents of `/etc/passwd`, to find
out the password of the `root` user.

## Shodan Webcam Research

We did some recon through Shodan and found many webcams given the "Server" header
of their HTTP server. We then used `nmap` to find suspicious open ports and
tried to guess their passwords while browsing their login page.

## Terms

Pentesting, Bug Bounty, Full Disclosure, Responsible Disclosure, Fingerprinting
WAF - Web Application Firewall, Botnet, Bot Herder, IOC - Indicator of Compromise.

## Homework
1. Do HTML Dog's Beginner, Intermediate and Advanced HTML tutorials: [http://www.htmldog.com/guides/html/](http://www.htmldog.com/guides/html/).
You can also do the CSS ones: [http://www.htmldog.com/guides/css/](http://www.htmldog.com/guides/css/).

2. Watch Mr. Robot.

3. Practice with https://www.typingclub.com. Reach at least 55WPM.

4. Research and public speaking; find a topic - either a technologoy (e.g. DNS, DHCP)
or a security-related news article and prepare a 2-3 minute talk about it.

5. FOLLOW YOUR FELLOW CLASS MATES: http://bit.ly/2B87gDw with your Twitter, Github and Linkedin.

6. Use the following `nmap` command: `$ sudo nmap -PN -sS -p80 <ip address>`
and sniff the communications with Wireshark, save it as a `.pcap` file.

7. Research your own local LAN devices with `nmap` and try to find vulnerabilities
around you :).

<hr>
Copyright 2019 Sagi Kedmi
