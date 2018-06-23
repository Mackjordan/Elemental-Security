# Authentication Controls

##### Knowledge
* Something a user knows
* Password / Pass-phrase / PIN

##### Possession  
* Something a user has
* Token, Smartcard

##### Biometric
* Something a user is, Something a use does
* Physiological, Behavioral

| Type | Security features | Specific Use |
|------|-------------------|--------------|
| Smart Card | Embedded chip and one or more certificates | N/A |
| Common Access Card (CAC) | Smart card that includes a picture of the user. Used for both visual identification and computer access. | Department of Defense. |
| Personal Identity Verification (PIV) | Smart card that includes a picture of the user. Used for both visual identification and computer access. | Federal Agencies |
| Contactless Card | Contactless smart card that can be read without inserting into a reader device. (Read range 1-3”) | N/A |
| Proximity Card | Contactless smart card that can be read without inserting into a reader device. (Read range up to 15") | N/A |


### Password / PIN Controls
Layered password controls include:
* Strength, complexity, limited login attempts, and aging
* Hashing, hashing with salt, and encryption
* User training
Even with the above controls, passwords alone provide minimal protection and are considered the weakest form of authentication.

### Tokens
A token can be a hardware device or embedded software that is in the user’s possession.
* Implementation requires authentication server and distribution of hard or soft tokens.

### HMAC—based One-Time Password algorithm (HOTP)
HOTP incorporates a secret key, a counter (hardware or software token), and a cryptographic hash function to create a One-time Password (OTP).
* The hash is different every time.
* The OTP is used once and never again.
* Security can be enhanced by adding a PIN.

### Time-based One-Time Password (TOTP)
TOTP incorporates a secret key, the current time of day, and a cryptographic hash function. TOTP has a short life - typically 30-60 seconds
* The authenticator app is configured ahead of time (which includes the secret key).
* Timestamps usually increment every thirty seconds.
* The TOTP is sent to the server and compared with a server generated TOTP.
* Used by Google and Facebook.

### Smartcards
A smartcard is a card/badge that is in the user’s possession. Smartcards can be used as ID badges as well as for building access and network authentication.
* Implementation requires a smartcard management system which includes customization, issuance, revocation, and replacement.

### Biometrics
Biometric options include fingerprint scanner, retinal scanner, iris
scanner, voice recognition, and facial recognition.
* Accuracy and acceptance are the most significant implementation challenges.

### Biometric Adoption
Biometric systems are the most trustworthy (even more so when combined with another factor); however, adoption has been influenced by cost, enrollment time, and user acceptance. During the enrollment process, the biometric registration system takes multiple measurements and goes through a series of validation processes.
* The measurements are either hashed or encrypted.
* Biometric systems may inadvertently detect drug usage, illness, and pregnancy.
