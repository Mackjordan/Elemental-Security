# Hashing
Hashing produces a visual representation of a data set.

1. Variable Length Input
2. Hash Function
3. Unique One—way Fixed. Length Output. (Fingerprint)

* The original message remains intact.

### Hashed MAC
A hashed message authentication code (HMAC) is a hashed value that includes a symmetric key.
* An HMAC cannot be reproduced without knowing the key.
* An HMAC provides integrity and data origin authentication.
* HMAC is used by cryptographic protocols such as the TLS and lPsec to verify the integrity of transmitted data during secure communications.

### Hashing Use Cases
The objective of hashing is proving integrity.
* Validate that a message has not been changed during transmission (message digest).
* Verify that a file has not been altered (checksum).
* Verify that a forensic clone is intact.

### Hash Algorithm Characteristics
In order to be considered secure, cryptographic hash functions must meet three criteria.
* Output must not be reversible (one-way representation).
* Variable length input must produce fixed length output.
* Output must be unique to the input. If an algorithm produces the same value for two different inputs, the result is known as a collision.

### Hashing Algorithms
##### Message Digest (MDx)
* MD5 has been shown to be subject to collisions attacks and is ”broken”

##### Secure Hash Algorithm (SHA)
* Created by the NSA
* SHA-l has been shown to be subject to collision attacks.
* SHA-Z family is widely used and includes SHA-256, SHA-384, and SHA—SlZ

##### RIPEMD
 * RIPEMD was based on MD4; it has been replaced by RIPEMD-160

### Message Digest in Action
1. Alice puts message through a hashing algorithm and generates a message digest (Hash) value.
2. Alice sends message and message digest to Bob.
3. Bob receives the message and message digest.
4. Bob puts message through a hashing algorithm and generates a message digest (hash) value.
5. Bob compares both message digests.
6. If the message digests are the same, the message was not modified in transmission.
7. If the message digests are different, the message was modified in transmission.


### Rainbow Tables & Salting
Rainbow tables are publicly available tables of precomputed hashes.
* Salts are values appended to the input to negate the value of rainbow tables.

| User | Password | Salt  | Hash Input |
|-----|------------|-------------|-----------------------|
| Bob | Password99 | 8fjhr9$k40$ | Password998fjhr9$k40$ |
| Mary | Password99 | K94lf88fe2 | Password99K94lf88fe2 |
