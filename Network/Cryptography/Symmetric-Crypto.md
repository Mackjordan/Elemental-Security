# Symmetric Encryption
Symmetric means the same key is used to encrypt and decrypt.
* Symmetric key may be referred to as single key, shared key, or session key.
* The key dictates what parts of the algorithm will be used, in what order, and with what values.
* The goal of Symmetric encryption:
1. Cleartext
2. Cipher + Key(Shared Key)
3. Ciphertext
4. Cipher + Key(Shared Key)
5. Cleartext


### Symmetric Ciphers
| Type | Method  | Algorithms |
|------|---------|------------|
| Stream Cipher | Works with one bit at a time | RC4 |
| Block Cipher | Works with blocks of data | DES, 3DEC, AES, Blowfish, Twofish, IDEA |


### Block Cipher Modes  
######  Electronic Codebook (ECB)
ECB Mode each block is independent (doesn’t hide patterns. Not suitable for long messages).

##### Cipher Block Chaining (CBC)
CBC Mode includes an initialization vector (IV) and a component of the previous Ciphertext to leverage randomization.

##### Counter (CTR) Mode
CTR does not have any dependencies. Requires synchronous counters at sender and receiver. Converts block Cipher to a stream Cipher using XOR functions.

##### Galois/Counter Mode (GCM)
GCM is a very efficient mode of operation for symmetric key cryptographic 128-bit blocks. GCM can take advantage of parallel processing.


### Stream Cipher Components
##### Input
* Plain text

##### Keystream
Set of random values (should be as long as the plaintext/ non-repeating)
* True Random Number Generators (TRNGs)
* Pseudorandom Number Generators (PRNGs)
* Cryptographlcally Secure Pseudorandom Number Generator (CSPRNG)
* Designed to resist attempts by a attacker to predict its next output
* Random and unpredictable

##### Function
XOR operation:

> 1+1=0, 0+o=0, 1+0=1, 0+1=1

Input:

> 10011100101010

Keystream:

> 00011010001110

Output:

> 10000110100100


### Symmetric Algorithm
##### Data Encryption Standard (DES)
64-bit key size / 16 rounds of substitution and transposition.
* 1977 established a US Government standard.
* 1998 demonstrated that it could be ”broken” in less than 56 hours.

##### Triple DES (3DES)
64-bit key / 48 rounds of substitution and transposition using either 2 or 3 keys.
* 1999 replaced DES as a US Government standard.
* Considered deprecated.

##### Advanced Encryption Standard (AES) Standard (Rijndael)
128- or 192- or 256-bit key/ 10 or 12 or 14 rounds of substitution and transposition
 * 2002 replaced 3DES as a US Government standard

##### Others to recognize as:
Blowfish, IDEA (used on PGP), Twofish (open source), RC4 (stream cipher)
