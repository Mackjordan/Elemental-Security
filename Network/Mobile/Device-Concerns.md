# Mobile Device Concerns
The upside of mobile device use is communication, social
engagement, and productivity.
The downside is inadvertent or malicious circumvention of
company policies, misuse of features/functionality, and threat
exposure.
* MDM solutions can monitor activity and enforce rules.

### Device-related concerns

##### Custom firmware (ROM)
Custom firmware is firmware for a device that has been altered from the original factory settings. This firmware can bring added functionality, but it can also result in security holes. Custom firmware should be used only on devices that do not have access to critical information. Custom firmware usually have all the extra restrictions removed, enabling users to sideload apps, tether their mobile data connection to their computer without paying extra for it, gain root access, use their device in any region etc. without any need for circumventing the protection themselves.

##### Firmware OTA updates
Firmware essentially is software. Firmware over-the-air (OTA) updates is a method for distributing firmware or software updates to a mobile device in contrast to having to go to a specific service center to have updates installed. Firmware may be stored in a chip, but like all software, it sometimes requires updating. Firmware OTA (over the air) updates are a solution to this problem. Similar to adding or updating an app from an app store, you can tap a menu option on a mobile device to connect to an app store and update the device firmware. 

### APP-related Concerns
##### Third-party APPs
Multiple definitions for third-party APPs.
* APPs that are provided by a vendor other than the manufacturer of the device (e.g. camera APP).
* Plug-in to software (may be authorized or unauthorized).
* Applications that have not been approved or vetted by the device manufacturer.

##### Jailbreaking (Apple)
Jailbreaking is the bypass of several types of Apple prohibitions for the end user including installing non-approved APPS via sideloading. Jailbreaking is a process by which the user escalates their privilege level, bypassing the operating system’s controls and limitations. The user still has the complete functionality of the device, but also has additional capabilities, bypassing the OS-imposed user restrictions. There are several schools of thought concerning the utility of jailbreaking, but the important issue from a security point of view is that running any device with enhanced privileges can result in errors that cause more damage, because normal security controls are typically bypassed.

##### Rooting (Android)
Attaining privileged control (root) over the device operating system including the ability to modify settings and run specrallzed APPs. Rooting a device is a process by which OS controls are bypassed, and this is the term frequently used for Android devices. Whether the device is rooted or jailbroken, the effect is the same: the OS controls designed to constrain operations are no longer in play and the device can do things it was never intended to do, good or bad.

##### Sideloading
Sideloading is the process of adding apps to a mobile device without using the authorized store associated with the device. Currently, sideloading only works on Android devices, as Apple has not enabled execution of any apps except those coming through the App Store. Without Jailbreaking. Sideloading is an alternative means of instantiating an app on the device without having to have it hosted on the requisite app store. The downside, simply put, is that without the vendor app store screening, one is at greater risk of installing malicious software in the guise of a desired app.

##### Third-Party App Stores
Many mobile devices have manufacturer-associated app stores from which apps can be downloaded to their respective devices. These app stores are considered by an enterprise to be third-party app stores, as the contents they offer come from neither the user nor the enterprise in nature. Currently there are two main app stores, the Apple App Store for iOS devices and Google Play for Android devices. The Apple App Store is built on a principle of exclusivity, and stringent security requirements are highly enforced for the apps that are offered. Google Play has fewer restrictions, which has translated into some security issues stemming from apps. Managing what apps a user can add to the device is essential because many of these apps can create security risks for an organization. This issue becomes significantly more complex with employee-owned devices and access to corporate data stores. The segmentation options discussed earlier to separate work and personal spaces are offered on a limited number of mobile devices, so the ability to control this access becomes problematic. Virtually all segmentation is done via an additional app, the MDM solution. Devices permitted access to sensitive corporate information should be limited to company-owned devices, allowing more stringent control.

### Feature-related Concerns
| Concern | Description |
|---------|-------------|
| Camera | Unauthorized use (take pictures or watch user)|
| SMS / MMS | Bypass of normal communication channels.|
| External media | Unauthorized transfer of data or programs. |
| USB OTG (0n the go) | Unauthorized connection master/slave to a USB device (e.g. camera)|
| Recording Mic | Unauthorized use (recording or listen to user). |
| GPS Tagging | Location exposure. |
| WiFi connection | Unauthorized connection to a hostile or exposed network. |
| Tethering | Unauthorized use of a device as a hotspot. |
| Payment methods | Connecting to NFC (e.g. Apple Pay), or WAP (e.g. Google Wallet)|
