# Digital Signature
A digital signature is a message digest that has been encrypted using a private key.

### Digital Signature Use Case
The goal of a digital signature integrity and non-repudiation
* Integrity is the assurance that the data has not been modified.
* Non-repudiation means that the signer cannot deny sending the message. Conversely, the receiver can trust that the message came from the named signer.

### Cryptographic Objectives
* A message can be hashed, which provides for integrity.
* A message can be digitally signed, which provides for non-repudiation and integrity.
* A message can be encrypted, which provides for confidentiality.
* A message can be encrypted and digitally signed, which provides for confidentiality, non-repudiation, and integrity.

### Digital Signature Algorithms
__NOTE: Digital signatures require two algorithms—a hashing algorithm and a digital signature algorithm.__
##### RSA
Widely implemented
* Defacto commercial standard
* Works with both encryption and digital signatures

##### Digital Signature Algorithm (DSA)
* Published by NIST in cooperation with the NSA. US Government Digital Signature standard.

### Digital Signature in Action

1. Alice puts a message through a hashing algorithm and generates a message digest(Hash) value.
2. Alice encrypts the message digest with her PRIVATE value.
3. Alice sends plain text message and message digest to Bob.
4. Bob receives the message and the message digest.
5. Bob decrypts the message digest using Alice's PUBLIC key proving authenticity (Non-repubiation)
6. Bob puts the plain text message through the same hashing algorithm and generates a message digest.
7. Bob compares both messages digests.
8. If the message digests are the same-the message was not modified in transmission (Integrity).
9. If the message digests are different- the messages was modified in transmission.
