# Cryptographic Attacks
A cryptographic attack is a method for circumventing the security of a cryptographic system by finding a weakness in a code, cipher, cryptographic protocol, or a key management  scheme.
* This process is also called "cryptanalysis".

### Crypto Attack Categories  
Intention is to break a cryptosystem and find the plaintext from the ciphertext. The attacker’s objective is to identify the key.

### Crypto Attack Categories
| Object | Description |
|--------|-------------|
| Known ciphertext | A sample of ciphertext is available without the plaintext associated with it. |
| Known Plaintext | A sample of ciphertext and the corresponding known plaintext is available. |
| Chosen Plaintext | Can choose the plaintext to get encrypted and obtain the corresponding ciphertext. |
| Chosen Ciphertext | Can select the ciphertext and obtain the corresponding plaintext.|

### Key Attacks
| Attack   | Description |
|----------|-------------|
| Brute Force | Every possible key is tested (online/offline). |
| Dictionary | List of known keys tested. |
| Frequency | Looking for patterns to reveal the key. |
| Replay | Attacker tries to repeat or delay a cryptographic transmission. |


### Hash Attacks
###### Collision
Using brute force to find two inputs producing the same hash value.

###### Birthday
Exploits the mathematics behind the birthday problem in probability theory
to cause a collision.
* How many people must be in the same room for the chance to be greater than even that another person has the same birthday as you = 253.
* How many people need to be in the room for the chance to be greater than even at least two people share a birthday = 23
* Any random set of 23 >= 50% chance

###### Rainbow
Table Comparing a table of known inputs/outputs to unknown outputs.

### Downgrade Attack
A downgrade attack is an attack on a system or communications protocol that forces degradation to a lower-quality crypto mode (if available) designed for backward compatibility.
* The 2014 POODLE attack took advantage of the option resulting in client fallback to SSL 3.0.

### Weak Implementation
Attackers take advantage of misconfigurations, weak keys, broken or deprecated versions.
* Deprecated means that the use of the algorithm and key length is allowed, but the user must accept some risk (weakness).
* Broken means that the algorithm and/or key length is exploitable.
