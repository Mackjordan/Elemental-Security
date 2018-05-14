# Hardware / Firmware Security Components

| Acronym | Description |
|---------|-------------|
| FDE / SED | Full disk encryption/self-encrypting drives |
| TPM | Trusted platform module |
| HSM | Hardware security module |
| UEFI / BIOS | Unified Extensible Firmware Interface |
| Secure Boot | Secure Boot |
| RoTs | Roots of Trust |

### Hardware Encryption
Full disk encryption (FDE) / self—encrypting drives (SED) is a hardware-based mechanism for automatically encrypting all data written to the magnetic media.
* Factory set encryption (circuit built into the disk drive controller chip)
* Drive powers up locked
* Key is never present in memory
* Transparent to the user with the exception of required boot-up password
* Does not effect performance
* Use case: Securing data at rest

### A trusted platform module (TPM)
TPM is a special hardware chip installed on a computer’s motherboard that is responsible for protecting passwords, symmetric and asymmetric keys, hashes, and digital certificates that are specific to that system hardware.
* The chip contains an RSA key used for encryption and
authentication
* TPMs are compatible with most operating systems
* Use case: Encrypting hard drives independent on the drive itself
* Use case: Storing passwords and other keys independent of the operating system

### A hardware security module (HSM)
HSM is a physical device whose function is secure cryptoprocessing.
* HSMs take the form of adapter cards, USBs, or network attached devices
* HSMs can be clustered for high availability
* Fast, scalable, and expensive
* Use case: Used for encryption during secure login/authentication processes, during digital signings of data (e.g. certification authority), and for payment security systems (e.g. ATMs)

### Unified Extensible Firmware Interface (UEFI)
UEFI / BiOS is an open standard interface layer between the firmware and the operating system that requires firmware updates to be digitally signed.
* Designed as a replacement for traditional PC BIOS
* Additional functionality includes support for Secure Boot, network authentication, and universal graphics drivers
* Use case: Protects against BIOS malware attacks including rootkits

### Roots of trust (RoTs)
RoTs are hardware / software components that perform foundational security functions (e.g. protect keys, perform device authentication, verify digital signatures).
* Because roots of trust are inherently trusted and must always behave in an expected manner, they must be secure by design.
* Ideally implemented in hardware or protected by hardware.
* As the first code that executes at power-on, boot firmware by default is a root of trust.
* Use case: In development — securing mobile devices/verifying the integrity of the device.
