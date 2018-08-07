#Apple iOS 
iOS (formerly iPhone OS) is a mobile operating system created and developed by Apple Inc. exclusively for its hardware. It is the operating system that presently powers many of the company's mobile devices, including the iPhone, iPad, and iPod Touch. It is the second most popular mobile operating system globally after Android. Originally unveiled in 2007 for the iPhone, iOS has been extended to support other Apple devices such as the iPod Touch (September 2007) and the iPad (January 2010). As of January 2017, Apple's App Store contains more than 2.2 million iOS applications, 1 million of which are native for iPads. These mobile apps have collectively been downloaded more than 130 billion times.


### Carrier Unlocking
Unlocking an iPhone allows the iPhone to be used with any wireless carrier using the same GSM or CDMA technology for which the particular phone model was designed to operate. Initially most wireless carriers in the US did not allow iPhone owners to unlock it for use with other carriers. However AT&T allowed iPhone owners who have satisfied contract requirements to unlock their iPhone. Instructions to unlock the device are available from Apple, but it is ultimately the sole discretion of the carrier to authorize the device to be unlocked. This allows the use of a carrier-sourced iPhone on other networks. Modern versions of iOS and the iPhone fully support LTE across multiple carriers despite where the phone was originally purchased from. There are programs to remove SIM lock restrictions, but are not supported by Apple and most often not a permanent unlock – a soft-unlock.

### Jailbreaking

Since its initial release, iOS has been subject to a variety of different hacks centered around adding functionality not allowed by Apple.[144] Prior to the 2008 debut of Apple's native iOS App Store, the primary motive for jailbreaking was to bypass Apple's purchase mechanism for installing the App Store's native applications. The general motives for jailbreaking have changed. People jailbreak for many different reasons, including gaining filesystem access, installing custom device themes, and modifying SpringBoard. An additional motivation is that it may enable the installation of pirated apps. On some devices, jailbreaking also makes it possible to install alternative operating systems, such as Android and the Linux kernel. Primarily, users jailbreak their devices because of the limitations of iOS. Depending on the method used, the effects of jailbreaking may be permanent or temporary. Apple claimed that it will not release iOS software updates designed specifically to break these tools (other than applications that perform SIM unlocking); however, with each subsequent iOS update, previously un-patched jailbreak exploits are usually patched.


### Legality of Jail breaking
In 2010, the Electronic Frontier Foundation (EFF) successfully convinced the U.S. Copyright Office to allow an exemption to the general prohibition on circumvention of copyright protection systems under the Digital Millennium Copyright Act (DMCA). The exemption allows jailbreaking of iPhones for the sole purpose of allowing legally obtained applications to be added to the iPhone. The exemption does not affect the contractual relations between Apple and an iPhone owner, for example, jailbreaking voiding the iPhone warranty; however, it is solely based on Apple's discretion on whether they will fix jailbroken devices in the event that they need to be repaired. At the same time, the Copyright Office exempted unlocking an iPhone from DMCA's anticircumvention prohibitions.

### Device Security
iOS utilizes many security features in both hardware and software. Below are summaries of the most prominent features.

##### Secure Boot
Before fully booting into iOS, there is low-level code that runs from the Boot ROM. Its task is to verify that the Low-Level Bootloader is signed by the Apple Root CA public key before running it. This process is to ensure that no malicious or otherwise unauthorized software can be run on an iOS device. After the Low-Level Bootloader finishes its tasks, it runs the higher level bootloader, known as iBoot. If all goes well, iBoot will then proceed to load the iOS kernel as well as the rest of the operating system.

##### Secure Enclave
The Secure Enclave is a coprocessor found in iOS devices that contain Touch ID or Face ID. It has its own secure boot process to ensure that it is completely secure. A hardware random number generator is also included as a part of this coprocessor. Each device's Secure Enclave has a unique ID that is given to it when it is made and cannot be changed. This identifier is used to create a temporary key that encrypts the memory in this portion of the system. The Secure Enclave also contains an anti-replay counter to prevent brute force attacks.

##### Passcode
iOS devices can have a passcode that is used to unlock the device, make changes to system settings, and encrypt the device's contents. Until recently, these were typically four numerical digits long. However, since unlocking the devices with a fingerprint by using Touch ID has become more widespread, six-digit passcodes are now the default on iOS with the option to switch back to four or use an alphanumeric passcode.

##### Touch ID
Main article: Touch ID
Touch ID is a fingerprint scanner that is embedded in the home button and can be used to unlock the device, make purchases, and log into applications among other functions. When used, Touch ID only temporarily stores the fingerprint data in encrypted memory in the Secure Enclave, as described above. There is no way for the device's main processor or any other part of the system to access the raw fingerprint data that is obtained from the Touch ID sensor.

##### Address Space Layout Randomization
Main article: Address Space Layout Randomization
Address Space Layout Randomization (ASLR) is a low-level technique of preventing memory corruption attacks such as buffer overflows. It involves placing data in randomly selected locations in memory in order to make it harder to predict ways to corrupt the system and create exploits. ASLR makes app bugs more likely to crash the app than to silently overwrite memory, regardless of whether the behavior is accidental or malicious.

##### Non-Executable Memory
iOS utilizes the ARM architecture's Execute Never (XN) feature. This allows some portions of the memory to be marked as non-executable, working alongside ASLR to prevent buffer overflow attacks including return-to-libc attacks.

##### Encryption
As mentioned above, one use of encryption in iOS is in the memory of the Secure Enclave. When a passcode is utilized on an iOS device, the contents of the device are encrypted. This is done by using a hardware AES 256 implementation that is very efficient because it is placed directly between the flash storage and RAM.

##### Keychain
The iOS keychain is a database of login information that can be shared across apps written by the same person or organization. This service is often used for storing passwords for web applications.

##### App Security
Third-party applications such as those distributed through the App Store must be code signed with an Apple-issued certificate. This continues the chain of trust all the way from the Secure Boot process as mentioned above to the actions of the applications installed on the device by users. Applications are also sandboxed, meaning that they can only modify the data within their individual home directory unless explicitly given permission to do otherwise. For example, they cannot access data that is owned by other user-installed applications on the device. There is a very extensive set of privacy controls contained within iOS with options to control apps' ability to access a wide variety of permissions such as the camera, contacts, background app refresh, cellular data, and access to other data and services. Most of the code in iOS, including third-party applications, run as the "mobile" user which does not have root privileges. This ensures that system files and other iOS system resources remain hidden and inaccessible to user-installed applications.

##### Network Security
iOS supports TLS with both low- and high-level APIs for developers. By default, the App Transport Security framework requires that servers use at least TLS 1.2. However, developers are free to override this framework and utilize their own methods of communicating over networks. When Wi-Fi is enabled, iOS uses a randomized MAC address so that devices cannot be tracked by anyone sniffing wireless traffic.

##### Two-Factor Authentication
Main article: Multi-factor authentication
Two-factor authentication is an option in iOS to ensure that even if an unauthorized person knows an Apple ID and password combination, they cannot gain access to the account. It works by requiring not only the Apple ID and password, but also a verification code that is sent to a device that is already known to be trusted. If an unauthorized user attempts to sign in using another user's Apple ID, the owner of the Apple ID receives a notification that allows them to deny access to the unrecognized device.
