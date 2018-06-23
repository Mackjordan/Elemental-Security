# Key Management
Key management describes the activities involving the handling of cryptographic keys and other related security parameters (e.g., passwords) during their entire lifecycle.
* This includes generation, exchange, storage, use, crypto-shredding (destruction) and replacement.
* A Key Management Practices Statement (KMPS) is a document that describes in detail the organizational structure, responsible roles and rules for key management.

### Cryptosystem Strength
A cryptosystem is only as strong as its weakest component.
* While many components of PKI are publicly known, private and symmetric keys must be appropriately strong.
* The strength of a key should be commensurate with the data/process protection requirements.
* The longer the key the stronger it is, the more processing power is required.

### Key Usage Best Practice
A key should only be used for one purpose (e.g. encryption).
* The use of the same key for different cryptographic purposes may weaken the security provided by one or both.
* Limiting the use of a key limits potential compromise damage.

### Key Update Best Practice
Because it increases any attacker's required effort, keys should be frequently changed.
* This also limits loss of information, as the number of stored encrypted messages which will become readable when a key is found will decrease as the frequency of key change increases.

### Perfect Forward Secrecy
Perfect Forward Secrecy (PFS) is an emerging protocol (set of rules) employed to ensure that if a private key was compromised, all previous uses of the key would remain secure. This effectively protects past sessions against future compromises.
* Perfect forward secrecy is achieved by using temporary key pairs to secure each session—they are generated as needed, held in RAM during the session, and discarded after use.

### Key Storage
Private keys must be securely stored. The measures taken to protect a private key must be at least equal to the required security of the use of the key.
* Centralized storage system refers to the use of a key management server (organizational control).
* Decentralized storage system refers to local key storage and management (user control).

### Hardware Security Module
A hardware security module (HSM) can be used to store cryptographic keys in tamper resistant hardware providing logical and physical protection.
* These modules traditionally come in the form of a plug-in card or an external device that attaches directly to a computer or network server

### Key Destruction
All copies of the private or symmetric keys should be irrevocably destroyed as soon as they are no longer required (e.g., for archival or reconstruction activity) in order to minimize the risk of a compromise.
