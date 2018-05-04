# Wireless Attacks


### Wireless Attacks
The objective of wireless attacks is the disruption, manipulation, or compromise of wireless transmission or devices.


### Wireless Attack Categories
| Category | Description |
|----------|-------------|
| Access | Authentication Exploit. - Enables unauthorized or unsolicited access to a end-user device.|
| Spoofing | Impersonating an wireless device. | Enables an attacker to as the trusted source and redirect/manipulate actions.|
| Sniffing | Capturing wireless data packets. - Enables an attacker to eavesdrop, manupuate, and/or reuse data packets.|
| Denial of Service | Overwhelming system resources. - Enables an attacker to make services unavailable for their intended use. |  

### Wireless Attack Concepts
| Category | Description |
|----------|-------------|
| War Driving | Scanning for unprotected wireless networks. |
| War Chalking | Marking a physical area to indicate a free, open, and/or insecure wireless network or access point. |

![SSID](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e6/Warchalking.svg/1000px-Warchalking.svg.png)

### Access Overview
> * Description: Authentication Exploit.
> * Outcome: Enables unauthorized or unsolicited access to a end-user device.
> ##### Bluejacking - Bluetooth Discovery
> * Enables an attacker to send unsolicited/unwanted message to a bluetooth device.
> ##### BlueSnarfing - Bluetooth Authentication.
> * Discovering and connecting to a bluetooth device with weak or non-existent authentication requirements.
> ##### NFC (Near Field Communication) Bump:
> * Enables an NFC-enabled attacker to connect to an NFC device by being in close enough range.

### Spoofing Overview
> * Description: Impersonating an wireless device.
> * Outcome: Enables an attacker to as the trusted source and redirect/manipulate actions.
> ##### Evil Twin - Rogue access point with the same SSID as authorized access point.
> * Enables an attacker to “trick” a user into connecting to a attacker controller network.
> * May also impersonate a “captive portal” to capture credentials and/or payment information.
> * Can be used as a stepping stone to a MiTM attack.

### Sniffing Overview
> * Description: Capturing wireless data packets.
> * Outcome: Enables an attacker to eavesdrop, manupuate, and/or reuse data packets.
> ##### Replay - Capturing and reusing packets.
> * Reusing authentication data/credentials.
> * Replaying the packet over and over causing a denial of Service.
> ##### IV (Initialization Vector) Attack - Capturing weak initialization vector (IV)
> * Knowledge of the IV can be used to decrypt data packets.
> ##### Wifi Protected Setup (WPS) Attack - Brute force identification of WPS PIN
> * Override the access point passphrase and gain access to the network.
> ##### RFID Eavesdropping - Intercepting communication between RFID Tags and Readers
> * Interception, manipulation, and reuse of data.

### Denial-of-Service Overview
> * Description: Overwhelming system resources.
> * Outcome: Enables an attacker to make services unavailable for their intended use.
> ##### Jamming - Overwhelming wireless frequencies with illegitimate traffic.
> * Frequency becomes unavailable for legitimate traffic.
> ##### Dissociation ( Also known as Deauthentication ) Attack - Spoofing a
> * disassociate message which forces a device to reassociate.
> * Device is continually “Knocked Offline”.
> * Can be used as a precursor to an Evil Twin attack.
