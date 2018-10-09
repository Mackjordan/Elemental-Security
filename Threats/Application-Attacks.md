# Application and Service Attacks

The objective of application and service attacks is the disruption, manipulation or compromise of network or host transmission, services, applications or data.


## Attack Categories
| Category | Description |
|----------|-------------|
| Spoofing | Impersonating an address, system, or person. - Enables an attacker to act as the trusted source and redirect/manipulate actions.|
| Poisoning | Manipulating trusted data (e.g. DNS) - Enables an attacker to manipulate trusted data for its purpose.|
| Hijacking | Intercepting communication between two systems. - Enables an attacker to eavesdrop, capture, manipulate, and/ or reuse data packets.|
| Denial of Service (DDos) | Overwhelming system resources - Enables an attacker to make services unavailable for their intended use.|
| Code | Exploiting weaknesses in server or client side code or applications. - Enables an attacker to take control.|

## Attack Concepts
| Category | Description |
|----------|-------------|
| Amplification: | An Amplification attack is where an attacker uses an amplification factor to multiply its power.|
| Privileged  Escalation: | Exploit designed to gain access to resources that are normally protected from an application or user.|
| Advanced Persistent Threat (APT): | An advanced persistent threat (APT) is a sophisticated attack in which an attacker gains access to a network and stays there undetected for a long period of time. |

## Spoofing
> * Description: Impersonating an address, system or person.
> * Outcome: Enables an attacker act as the trusted source and redirect/manipulate actions.
>
> ##### IP Address Spoofing
>* Using a trusted IP Address for Authentication.
>* Using a fake IP address to disguise the sender.
>* Using an Appropriate IP address to redirect an attack.
>
> ##### Mac (Media Access Control) Address spoofing.
>* Using a trusted MAC address for access.
>* Using a trusted MAC address to circumvent licensing.
>* Using a fake MAC address to mask the identity of a device.

## Poisoning
> * Description: Manipulating (altering ) a trusted source of data.
> * Outcome: Enables an attacker to manipulate trusted data for its own purposes.
Attacks to know.
> ##### ARP Cache Poisoning - MAC-to-IP address resolution.
> * Using a poisoned ARP cache to redirect traffic to a malicious host.
> * Using a poisoned ARP cache to stop traffic.
>
> ##### DNS Cache Poisoning - Domain / Host name-to-IP address resolution
> * Diverting website traffic to a malicious site.
> * Diverting website traffic to a non-existent site.

## HiJacking
> * Description: Intercepting communication between two systems
> * Outcome: An attacker intercepts communications between two systems.
> ### Hijacking - Common Attacks
> ##### Man-in-the-middle (MiTM) - Spoofing and/or poisoning
> * Exploiting real-time processing of transactions , conversations or data transfer.
>
> ##### Replay - capturing and reusing packets.
> * Reusing authentication data / credentials
> * Replaying the packet over and over causing a denial of service.
> ##### Man-in-the-Browser (MitB) - Internet version of MiTM
> * Manipulating the browser to control a session including what is displayed.
> ##### Session Hijacking
> * Stealing session cookies to “Take over” a user’s active session.
> ### Hijacking Web specific Attacks.
> ##### Domain Hijacking: Unauthorized modification of a domain name registration.
> * Using a legitimate website for malicious purposes
> ##### URL Squatting - Registering or using an internet domain name with bad faith intent to profit from the goodwill of a trademark belonging to someone else.
> * Directing users to fraudulent sites.
> ##### Typo Squatting - Taking advantage of a common typos to create fraudulent websites.
> * Redirecting users to malicious sites often to steal credentials or obtain personal information.
> #####  Click Jacking: Tricking user into clicking a button, picture or link.
> * Redirecting users to a malicious sites to download malicious code.

## Denial of Service (Dos)
> * Description: Overwhelming system resources.
> * Outcome: Resources become unavailable for their intended use.
> #####  DoS - Denial of Service - Transmitting malformed packets or unusual requests.
> * Shutting down a specific service or resource.
> #####  DDoS Distributed Denial of Service - Massive volume of service requests from multiple sources, often “Bots” configured in a botnet.
> * Shutting down a resource, and /or denying service to legitimate users.
> * Causing downstream degradation and /or malfunction of individual “bots”.


## Code
> * Description: Exploiting weaknesses in server or client side code or applications.
> * Outcome: Enables an attacker to take control.
> ##### Injection - tricking an application into including unintended commands.
> * Executing authorized commands or obtaining access.
> ##### Buffer Overflow - Writing excess data into system memory that overruns the buffer boundary an overwrites adjacent memory locations.
> * Executing authorized commands.
> #####  Skimming
> * Using a malicious “Shim” to manipulate an OS or application.
> #####  Refactoring - Reconstructuring code without changing external behavior.
> * Manipulating code with malicious intent.
> ###  Browser specific Attacks
> #####  Cross-Site Scripting: - Injection of malicious code that executes in a browser.
> * Resulting in session hijacking, reduction or bypassing access controls.
> ##### Cross-site Request Forgery: - Exploiting the trust relationship between a website and a browser.
> * Resulting in a unauthorized access and theft and/or credential modification.

## Zero-Day
> * A Zero-day: threat is the discovery of a previously unknown vulnerability for which there is no fix.
> * A zero-day attack occurs in the time period between when a exploit is developed and when a patch has been developed and when a patch has been released or a compensating control identified. 

