# 10/02/2018 - 6th Lecture

## `NETCAT`

We used `netcat` to create a lasting `tcp` server on port `1234` with:

~~~
$ netcat -l 1234 -k
~~~

We then browsed to http://localhost:1234/ and saw the HTTP request that our
browser sent inside netcat's terminal.

## Pipes

We used `cat <file>` to print a file's content to `stdout`. We then used pipe
to channel the stdout one program to another.

For instance,

~~~
$ cat baba.html | hexdump
~~~

Would show us the hexdump of the file `baba.html`.

We also learned about CRLF (Carriage Return / Line Feed) and their `ascii`
representations.

We noted that Linux uses only LF (0x0a) for newines while Windows uses
CRLF (0x0d 0x0a).

## VLANs

We understood why and how VLANs are used within a network topology.

VLANs use 802.1q Ethernet tagging in order to "paint" a packet with a specific
VLAN. VLANs can spread over different switches. Each VLAN has it's own
default gateway.

We understood that Broadcast Storms may happen with some network topologies
and that the solution is employing a protocol that is called "Spanning Tree"
(STP).

## HTTP

We understood what are HTTP methods (e.g. GET / POST), HTTP paths (e.g. "/index.html", "/images/baba.png"),
and HTTP headers

## Web Servers

We understood the basics of HTTP. We understood the role of a Web server,
such as apache or nginx.

We installed apache on a Ubuntu machine with:

~~~
$ sudo apt install apache2
~~~

We verified with `netstat` that there is program with the name "apache" that
listens on TCP/80:

~~~
$ netstat -ltnp
~~~

Then we used `cd` to change our current directory to `/var/www/html`, and
created a new file there: `gedit baba.html`.

We then wrote simple HTML in `baba.html` and opened Chrome with
"http://localhost/baba.html"

We saw how we can use `CSS` to create better looking web sites.

## APIs

We understood what are APIs, how they're used by different companies to
consume the services of other companies.

We also noted that many companies use internal APIs in the form of "Microservices".

We understood the difference between Monoliths and Microservices.

## Linux Commands

- `cd` - change directory, e.g. `cd /var/www/html`.
- `ls` - list files in current directory.
- `pwd` - print working directory.
- `cat <flie>` - print file content to stdout.

## Terms

Cryptojacking,  stdout, hexdump, Markdown.

## Homework

1. Do HTML Dog's Beginner, Intermediate and Advanced HTML tutorials: [http://www.htmldog.com/guides/html/](http://www.htmldog.com/guides/html/).
You can also do the CSS ones: [http://www.htmldog.com/guides/css/](http://www.htmldog.com/guides/css/).

2. Watch Mr. Robot.

3. Practice with https://www.typingclub.com. Reach at least 55WPM.

4. Research and public speaking; find a topic - either a technologoy (e.g. DNS, DHCP)
or a security-related news article and prepare a 2-3 minute talk about it.

5. FOLLOW YOUR FELLOW CLASS MATES: http://bit.ly/2B87gDw with your Twitter, Github and Linkedin.

6. Find relevant job descriptions (e.g. SOC Analyst). Put them in Google Docs.
Highlight the different technologies that are required.

7. Review all previous lecture notes, make sure you understand what's going on -
if you aren't - Google it. If it doesn't help - make a list of questions for me
to answer :).

<hr>
Copyright 2019 Sagi Kedmi
