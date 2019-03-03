# 03/03/2018 - 12th Lecture

## Test #2 - Linux Command Line

We had our 2nd test!

## Public Key Encryption

We explained the elements of the Internet's PKI (Public Key Infrastructure)

We explained the difference between Symmetric Encryption (Shared Key) and
Asymmetric Encryption (Public Key Encryption).

We explained what are Digital Signature and how they're used by operating systems
and browsers to check if the certificate is valid (i.e. the certificate was signed
by a valid CA).

We also explained the role of CAs (Certificate Authorities).

We used Wireshark to capture and dissect a certificate.

## Python scripting

We explained the basics behind Python scripting. We used `Python`'s  `requests`
package to make `HTTP` requests.

```python
#!/usr/bin/python
import requests

r = requests.get('http://api.open-notify.org/astros.json')
print(r.text)
```

## Homework
1. Watch Mr. Robot.

2. Practice with https://www.typingclub.com. Reach at least 55WPM.

3. Prepare a 2-3 mins talk!

4. If you haven't done so already - create a CV using these templates: [https://docs.google.com/templates](https://docs.google.com/templates).
Bring it to me for review.

5. Start sending your CV to companies! The Job search begins! :)

6. Use OpenSSL to issue a Public / Private Key Pair. Encrypt something with
the private key. Decrypt it with the Public key. (Google it!)

7. Use Python to do a HTTP request to Chuck Norris random jokes: "https://api.chucknorris.io/jokes/random"

Use `pprint` to pretty print the JSON.

<hr>
Copyright 2019 Sagi Kedmi
