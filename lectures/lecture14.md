# 10/03/2018 - 14th Lecture

## Symmetric Encryption

### Block Ciphers
We talked about how block ciphers work. Example block ciphers are AES, DES and 3DES.

We also talked about the vulnerable ECB mode of operation and stated that
there are better modes such as CBC.

### Stream Ciphers

We talked about how stream ciphers work. Example stream ciphers are RC4 and Salsa20.


## CIA Triad and AAA

We explained the CIA - Confidentiality, Integrity and Availability and AAA -
Authentication, Authorization and Accounting.

[Click here for more info](https://www.hack2secure.com/blogs/an-introduction-to-core-security-concepts-cia-triad-and-aaa).


## Digital Signatures and Hashing

We talked at length about how digital signature are performed and used hash
functions such as SHA1 and SHA256 (`$ sha1sum`, `$ sha256sum`) and RSA
to create our own signature for a document - see homework!


We talked about rainbow tables as a way to reverse a hash.

We also talked about how people used to use hashing to store passwords in databases,
and that now the best practice is KDFs (Key Derivation Functions) such as bcrypt and scrypt.


## Python Scripting

We rigorously explained how to solve the Python homework.

## Homework
1. Watch Mr. Robot.

2. Practice with https://www.typingclub.com. Reach at least 55WPM.

3. Prepare a 2-3 mins talk!

4. If you haven't done so already - create a CV using these templates: [https://docs.google.com/templates](https://docs.google.com/templates).
Bring it to me for review.

5. Start sending your CV to companies! The Job search begins! :)

6. Digital Signature Exercise:
    1. Create a file named `plaintext` and added some data in it.

    2. Use OpenSSL to create a public / private RSA key pair.

    3. Use SHA256 to get a hash of `plaintext` and then encrypt it with the private key to get the signature.

    4. Send your neighbour the: `plaintext`, `public key` and `signature` for him to validate!

7.  Do [Google's Python's Class](https://developers.google.com/edu/python/)
please try to reach till "Dict and Files".

<hr>
Copyright 2019 Sagi Kedmi
