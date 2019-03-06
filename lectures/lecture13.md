# 06/03/2018 - 12th Lecture

## Binary Classification

We explained:

- True Positive (TP)
- False Positive (FP)
- True Negative (TN)
- False Negative (FN)

And that we may suffer from errors such as FPs and FNs when a security
product alerts (or doesn't) on something he deems wrong.

## Security Products / Techniques

We explained the following products:

- IDS/IPS (Snort)
- AV
- WAF
- Proxy (Forward, Reverse)
- HoneyPot (Deception)
- VPN
- FW
- Sandbox

## Once Again, We Explained Public Key Encryption

We explained the elements of the Internet's PKI (Public Key Infrastructure)

We explained the difference between Symmetric Encryption (Shared Key) and
Asymmetric Encryption (Public Key Encryption).

We explained what are Digital Signature and how they're used by operating systems
and browsers to check if the certificate is valid (i.e. the certificate was signed
by a valid CA).

We also explained the role of CAs (Certificate Authorities).

We used Wireshark to capture and dissect a certificate.

## OpenSSL

### How do I do public-key encryption with openssl?

OpenSSL is a public-key crypto library (plus some other random stuff).
Here’s how to do the basics: key generation, encryption and decryption.
We’ll use RSA keys, which means the relevant openssl commands are `genrsa`, `rsa`, and `rsautl`.

```
# Alice generates her private key `priv_key.pem`
openssl genrsa -out priv_key.pem 2048

# Alice extracts the public key `pub_key.pem` and sends it to Bob
openssl rsa -pubout -in priv_key.pem -out pub_key.pem

# Bob encrypts a message and sends `encrypted_with_pub_key` to Alice
openssl rsautl -encrypt -in cleartext -out encrypted_with_pub_key -inkey pub_key.pem -pubin

# Alice decrypts Bob's message
openssl rsautl -decrypt -in encrypted_with_pub_key -inkey priv_key.pem
```

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

6. Use OpenSSL and encrypt with symmetric encryption the following text: "attack at dawn".
Use the following ciphers: AES, RC4, DES, 3DES. Do a correctness test:

```
plaintext = decrypt(encrypt(plaintext, k), k)
```

7. Use Python to do a print random questions from: http://jservice.io/.

<hr>
Copyright 2019 Sagi Kedmi
