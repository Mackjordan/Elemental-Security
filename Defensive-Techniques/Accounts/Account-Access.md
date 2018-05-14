# Account Access

### AAA Primer
| Process | Description |
|---------|-------------|
| User (Subject) | Active entity requesting access. |
| Resource (Object) | Passive entity being accessed. |
| Identification | The process of ”claiming an identity" — who I say I am. |
| Authentication | The process of ”proving an identity” — verification of who I say I am. |
| Authorization | The process of granting an authenticated user access to a resource or permission to take an action. |
| Accounting | The process of tracking authenticated user activity and resource utilization. |

### User Name
Identification is the process of ”claiming an identity" which is generally expressed as a user name.
* User names should conform to an adopted naming convention (e.g. firstname.lastname@company.com)
* User names should be unique for accountability.
* User names should be non-descriptive of the user’s position or role.

### Authentication
Authentication is the process of ”proving an identity.” The proof is referred to as a factor. The combination of a user name and factors is referred to as credentials.

Types of factors include:
* Something a user nows.
* Something a user has in their possession.
* Something a user is (unique physiological characteristic).
* Something a user does.
* Somewhere a user is (location-based).

### Factor Requirements
##### Single—factor
* Only one factor is required for authentication.
##### Multi-layer
* Two or more of the same type of factor is required for authentication.
##### Multi-factor
* Two or more different types of factors are required for authentication.
##### Out-of-Band
* Use of more than one communication channels to required for authentication.

### Something You Know
Something you know is a shared secret known to the user and the authentication system.
* Passwords, pass-phrases, and PINS are data strings (letters, numbers, symbols)
* Cognitive passwords (challenge questions) utilize a preselected question and answer based on fact, opinion, or memory.
* Out-of-wallet passwords (challenge questions) are answers to questions derived from subscription databases.

### Something You Have
Something you have requires physical possession of a device.
* A secure token is a hand-held device with an LED that displays a number and the number is synchronized with an authentication server.
* A smart card is a credit card-sized card that has an integrated circuit and a certificate used to identify the holder.

### Something You Are
Something you are is a physiological characteristic.
* Biometric refers to ”human characteristics.”
* Physiological biometric markers include fingerprints, finger-scans, retina scans, iris scans, facial recognition, vascular patterns, palm scans, and hand geometry.

### Something You Do
Something you do is a behavioral trait.
* Behavioral biometric traits include voice pattern recognition, keystroke dynamics, and signature dynamics.

### Somewhere You Are
Somewhere you are is location-based — either physical or logical.
* A logical location is an IP address.

### Authentication Decisioning
Decisions regarding the type and number of factors should always be commensurate with the business value of what is being protected, regulatory requirements, and contractual obligations.
* Authentication controls should be subject to periodic risk assessments.
