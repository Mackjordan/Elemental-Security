# Digital Certificates
Digital Certificates are the mechanism used to generate a private key and to associate a public key with a collection of components sufficient to authenticate the claimed owner.
* The X.509 standard defines the certificate format and fields for public keys.
* The X.509 standard defines the distribution procedures.
* The current version of X.509 for certificates is v3.
* Certificate use object identifiers or Ole which are globally unambiguous persistent names.

### Public Key Infrastructure
Public Key Infrastructure (PKI) consists of programs, data formats, procedures, communication protocols, security policies, and public key cryptographic mechanisms working together in a comprehensive manner to enable secure communication.
* Public Key Infrastructure x.509 (PK/X) is the working group formed by the IETF to develop standards and models (known as x509).
* Public Key Cryptography Standards (PKCS) is a set of voluntary standards created by RSA and other industry leaders.


### x.509 v3 DI : Ital Certificates Fields
| Version | Serial Number | Signature | Issuer | Validity | Subject Name | Public Key | Issuer Unique ID | Subject Unique ID |
|-------|-------|-------|-------|--------|-------|-------|------|-----|
| Version # of the certificate | Unique identifier | Algorithm used to sign the certificate | Name of insurer | Valid date of certificate | Name of owner | Public key of named owner | ID of the Certificate Authority | ID of subject |

* Some certificates will include a Subject Alternate Name (SAN) that allows the owner
to specify additional host names (sites, IP address, common names)

### Types of Digital certificates (Use)
| Type |  User |
|------|-------|
| Personal | Verifies a user identity (generally used for email) |
| Server (Machine/Computer) | Verifies a device identity |
| Domain Validation | Wildcard certificate can be used with multiple subdomains of a domain (e.g. * .example.com) |
| Organization | Verifies a domain and a organization. |
| Extended Validation | Verifies a domain and a organization subject to additional vetting (a.k.a. "green bar" )|
| Code/ Object signing | Verifies origination/ownership as well as object integrity. |
| Trusted/Intermediate | Identifies root and intermediate Certificate Authorities. |


### Certificate File Extension and Formats
There are several certificate file extension types and encoding formats. They are specific to device/operating systems. For example, Windows uses .pfx files while Apache uses .pem, .crt and .cer. File types and formats can be converted.
* .pem (most common), .crt, .ca-bund/e, .cer, .p7b, .p7s files contain one or more X.509 digital certificate files that use base64 (ASCII) encoding.
* .pfx files are an archive file format for storing several cryptographic objects in a single file.

### Self—signed Certificate
A self-signed certificate is signed by the person creating it.
* The advantage is that there is no additional expense.
* The disadvantages is that a self-signed certificate can easily be impersonated, will present the user with a warning message and cannot be revoked.
* Use cases include a internal development server

### Trust Models (Chain of Trust)
* A Trust Model defines how users trust other users, organizations, CAs and RAs within the PKI.

###### Web of trust
* No central authority. Each user creates and signs their own certificate.
Users sign each others public key indicating ”trust”.

###### Third Part (Single Authority) Trust.
* A central third-party Certificate Authority (CA) signs a key and authenticates the owner.

###### Hierarchical
Extension of third party in which root CAs issues certificate to lower level "intermediate” CAs who can then issue certificates. Trust is inherited.
* Offline root CA is one that is isolated from a network and is often kept powered down to prevent compromise.
* A Registration Authority (RA) offloads some of the work from the CA. The RA can accept and process registration requests and distribute certificates.
* A Local Registration Authority (LRA) requires physical identification.

### Certificate Formats

###### PEM
Most common certificate format (Base64 encoded ASCII).
* Can include both the certificate and private key in one file or can be separate file
* Extensions include .pem, .crt, .cer,.key
* Use case: Apache

###### DER
Binary form of a PEM
* Extension include .cer, .der
* Use case: Java

###### P7B / PKCS#7
Contains certificate but not the private Key (Base64 encoded ASCII)
* Extensions include .p7b, .p7c
* Use case: Windows OS, Java Tomcat.

###### PFX/ PKCS#12
Contains certificate, intermediate certificate and private key (Binary)
* Extension include .pfx, .12
* Use case: Windows OS to import and export certs and keys


### Trusted Certificate Lifecycle
1. CSR - Certificate Signing Request (CSR).
2. Certificate is issued.
3. Certificate is published.
4. Certificate received.
5. Certificate if suspended / revoke or expired.
6. Key is destroyed.


### Certificate Pinning
Pinning is the process of associating a host with their expected X509 certificate or public key.
* A host or service's certificate or public key can be added to an application at development time, or it can be added manually upon first encountering the certificate or public key.
* Use Case: Pinning is intended to add a layer of security against Man-in-the-Middle attacks.


### Certificate Revocation
| Action  | Description  |
|---------------------------|----------------------------------------------------|
| Suspension | Temporary revocation of a certificate until a certificate problem can be resolved. |
| Revocation | Permanent withdrawal of trust by issuing authority before scheduled expiration date. |
| Certificate Revocation List CA (CRL) | maintained list of certificates that have been revoked. Pull model — CRL is downloaded by the user or organization. Push model — CRL is automatically sent out by the CA at regular intervals. |
| Online Certificate Protocol (OCSP) | Process designed to query the status of certificate in real-time. OCSP stapling is a time stamped (cached) OCSP response. |


### Certificate Expiration and Renewal
Certificate expiration dates are determined at time of issuance.
* Renewal is the responsibility of the owner. If renewal doesn’t happen, the certificate becomes invalid.
* Renewal options include maintaining the same key pair or generating new keys.
* The longer keys are in service—the more vulnerable they become.
