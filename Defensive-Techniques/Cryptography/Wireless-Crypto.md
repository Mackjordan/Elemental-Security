# Wireless Cryptographic Protocol

### Wireless Network Configurations
| Type | Description                                      | IEEE Standard     |
|------|--------------------------------------------------|-------------------|
| WPAN | Wireless Personal Area Network. A.K.A. Bluetooth | 802.15 standard. Interconnects devices Within a limited. range (e.g. keyboards) |
| WLAN | Wireless Local Area Network | 802.11 standard |
| WMAN | Wireless Metropolitan Area Network | 802.16 standard |
| WWAN | Wireless Wide Area Network | Point-to-point microwave links |


### 802.11 IEEE Standards
| Specification | Data Rate | Frequency | Distance |
|---------------|-----------|-----------|----------|
| 802.11  | 2 Mbps | 2.4 GHz | 100 m |
| 802.11b | 2 Mbps | 2.4 GHz | 140 m |
| 802.11a | 54 Mbps | 5 GHz  | 120 m |
| 802.11g | 54 Mbps | 2.4 GHz | 140 m |
| 802.11n | 150 Mbps | 2.4 / 5 GHz | 250 m |
| 802.11i | Security for 802.11 technologies |
| 802.11e | Quality of Service (QoS) for priority and time sensitive data. |

### Authentication Protocols
| Protocol | Description |
|----------|-------------|
| EAP Extensible Authentication Protocol (RFC 3748) | EAP is a authentication framework for wireless networks and P2P connections. |
| PEAP Protected Extensible Authentication Protocol | Encapsulates EAP in a TLS tunnel. Jointly developed by Microsoft, Cisco, and RSA. |
| EAP-FAST EAP-Flexible Authentication via Secure Tunneling | Lightweight implementation proposed by Cisco. |
| EAP-TLS EAP-Transport Layer Security | Defined in RFC 5216 is an open standard that uses TLS. Considered one of the most secure EAP standards. |
| EAP-TTLS EAP-Tunneled Transport Layer Security | Extends TLS (Client does not need to have a certificate legacy authentication is supported within a secure tunnel) |

### 802.11 Security
| Control | WEP | WPA | WPA2 |
|---------|-----|-----|------|
| Authentication | Preshared Key (PSK) or open | Enterprise RADIUS, Certificate or Personal PSK |  Enterprise RADIUS, Certificate or Personal PSK |
| Key | 64- or 128-bit key All users and services use the same key. | Separate keys (TKIP) 256—bit key | Separate keys 256—bit key and block size |
| Encryption | RC4 Stream Cipher | RC4 Stream Cipher |  AES Block Cipher |
| Integrity | 32-bit CRC Hash | 64-bit MIC | CCMP |
| Status | Insecure | Temporary fix Superseded by WPA2 | Current standard, Vulnerable if using Wifi, Protected Setup (WPS) |

### Wi-Fi Protected Setup
Created by the Wi-Fi Alliance and introduced in 2006, the goal was to make it easy to add new devices to an existing network without entering long passphrases.
* The PIN flaw allows a remote attacker to recover the WPS PIN in a few hours with a brute-force attack and, with the WPS PIN, the network's WPA/WPAZ pre-shared key.
* All WPS devices are vulnerable to unauthorized access if not kept in a secure area—an unauthorized user can connect by pressing the WPS button to command the router to make a WPS connection.


### Captive Portal
The captive portal feature is a software implementation that blocks clients from accessing the network until user verification has been established.
