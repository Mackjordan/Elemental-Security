# Cryptography Basic
Cryptography is the science of secret writing that enables an entity to store (data-at-rest), transmit data (data—in-transit), and process (data-in-use) in a form that is only available to an intended recipient.
* A modern cryptosystem is the hardware and/or software implementation of cryptography.

### Use Cases
Primary cryptographic use cases and corresponding techniques include:
* Confidentiality (encryption)
* Integrity (hashing)
* Non-repudiation (digital signatures)
* Authentication (digital certificate)
* Obfuscation (encryption, steganography)

### Cryptographic Terminology Primer
| Term   | Description   |
|--------|---------------|
| Plaintext (cleartext) | Human readable text |
| Ciphertext | Encrypted and/or human unreadable text |
| Cipher | A technique that transforms plaintext into Ciphertext and back to cleartext.|
| Algorithm | A cryptographic algorithm is a mathematically complex modern cipher. |
| Stream Cipher | Algorithm that works with one bit at a time |
| Block Cipher | Algorithm that works with blocks of data |

### Cryptographic Terminology
|  Term  |  Description |
|--------|--------------|
| Key/ Cryptovarlable | Secret value used with an Algorithm. The key dictates what parts of the algorithm Will be used, In what order, and with what values. |
| Key Space | Number of possible key combinations.  e.g. 256-bit = 2 to the 256 power = 1.1578 x 1077 possible keys. |
| Key Stretching | Technique to strengthen a weak key (password) and protect against brute force attacks by feeding the initial key into an algorithm (e.g. PBKDFZ, bcrypt) that outputs a enhanced key. |
| Symmetric | Using a single key. |
| Asymmetric | Using two mathematically related keys (public/ private). |
| Ephemeral Key | Temporary key generated for a connection and never used again. |

### Cipher techniques
| Technique   |  Description    |
|-------------|-----------------|
| Substitution cipher | Substitution cipher replaces one character or bit for another character or bit. The key is the shift pattern. ROT13 is a Simple letter substitution that replaces a letter with the letter 13 after it in the alphabet. |
| Transposition Cipher | Transposition cipher moves characters or bits to another place within the message block. The key is the transposition code.
| Confusion | Confusion is the process of changing the values. Complex substitution functions are used to create confusion. |
| Diffusion | Diffusion is the process of changing the order. Sending bits through multiple rounds of transposition is used to create diffusion. |

### Lightweight cryptography
The majority of modern cryptographic algorithms were designed for desktop/server environments. Many of these algorithms cannot be implemented in resource constrained devices (e.g. automotive systems, Internet of Things (IoT), smart grid).
* Emerging lightweight cryptographic algorithms are being developed to support low power devices as well as low latency and high resiliency requirements.

### Strength & Workfactor
Strength of a cryptosystem is a combination of the algorithm, the algorithmic process, the length of the key, and the secrecy of the key. If one element is weak, the cryptosystem can potentially be compromised.
* The workfactor is the amount of time and effort it would take to penetrate (break) a cryptosystem.
* Deprecated means that the use of the algorithm and key length is allowed, but the user must accept some risk (weakness).
* Broken means that the algorithm and/or key length is exploitable.
* Stronger the cryptosytem > processing power required.

### Security through Obscurity
Security through obscurity is the reliance on the secrecy of the design or implementation as the main method of providing security for a system or component of a system.

### Steganography
Steganography is the science of hiding information.
* The goal of cryptography is to make data unreadable; the goal of steganography is to conceal.
* Digital steganography is the practice of concealing a file within another file.
* Hidden binary files are most often found embedded in image and audio files

### Steganography Use Cases
The objective of Steganography is concealment.
* A digital watermark is a hidden message that is used to prove or claim ownership (generally intellectual property or an artistic work).
* Conceal malicious code (malvertising, phishing, exploit kits)
* Covert communication
