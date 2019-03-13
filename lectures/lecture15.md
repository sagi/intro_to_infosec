# 13/03/2018 - 15th Lecture

## Cryptography Revisited

We talked about symmetric encryption, hashing and asymmetric encryption.

### Hashing

We talked about cryptographic hashes (MD5, SHA1, SHA256) and KDFs (Key Derivation Functions).

We visualized how KDFs make it way harder for attackers to derive passwords, even if
the database is exfiltrated

### Symmetric Encryption

We talked about how symmetric encryption works (e.g. AES) and how we can use
Message Authentication Codes (MACs) to authenticate ciphertexts and avoid
tampering by MiTMs.

### Public Key Cryptography Revisited

We explained, once again, at length, public key crypto. We understood the difference
between encrypting and signing.

We encrypt with the public key when we want the ciphertext to be decrypted by the holder of the private key.

We "encrypt" (sign) with private key when we want the "ciphertext" (signature) to be decrypted ("verified") by **any** holder of the public key.

#### Sign a Random Plaintext

```sh
# Generate a plaintext with random bytes

head -n 2 /dev/urandom | base64 > plaintext

# Generate an RSA private and publikey and pu

openssl genrsa -out priv_key.pem 2048
openssl rsa -pubout -in priv_key.pem -out pub_key.pem

# Get plaintext's hash

sha256sum plaintext | cut -d' ' -f1 > plaintext_hash

# Sign plaintext's hash

openssl rsautl -sign -inkey priv_key.pem -in plaintext_hash -out plaintext_hash_signed
```

### Verify a Signed Plaintext

We only need the plaintext, public key and the signature

```bash
# Verify plaintext's signature

openssl rsautl -verify -pubin -inkey pub_key.pem -in plaintext_hash_signed

# Check that the output from the above command is equal to:

sha256sum plaintext
```

## Terms

Social Engineering, One Way Function, Rainbow table, Key Derivation Function,
Bitflip, Tampering, CTF - Capture The Flag.

## Python Scripting

We rigorously explained how to solve the Python homework.

## Homework
1. Watch Mr. Robot.

2. Practice with https://www.typingclub.com. Reach at least 55WPM.

3. Prepare a 2-3 mins talk!

4. If you haven't done so already - create a CV using these templates: [https://docs.google.com/templates](https://docs.google.com/templates).
Bring it to me for review.

5. Start sending your CV to companies! The Job search begins! :)

6. **STUDY FOR TEST!** - 24/03/2019 - study from lecture 11 (including) and from the "Defense and Offense" in the course's Google Drive

8.  Do [Google's Python's Class](https://developers.google.com/edu/python/)
please try to reach till "Dict and Files".

<hr>
Copyright 2019 Sagi Kedmi
