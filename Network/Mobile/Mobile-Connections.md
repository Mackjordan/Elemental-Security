# Mobile Connection Methods

Mobile Device
A mobile device is a generic term for any communication device
that is portable.
* A laptop is an all-in-one personal computer that can easily be
moved and used in a variety of locations. Laptops use the same
operating systems as desktops.
* A tablet is a touchscreen device that has thin flat form factor.
Tablets require specialized operating systems.
* A smartphone is pocket-sized touchscreen device that
incorporates traditional cell phone features. Smartphones
require specialized operating systems

### Connection Methods
| Method | Description |
|--------|-------------|
| Cellular | Radio frequency distributed network |
| WiFi | Radio frequency contained network |
| SATCOM | Satellite communications network |
| Bluetooth | Shortwave network |
| NFC | Nearfield communications network |
| ANT | ”Wearables” sensor network |
| IR | Optical short-wave network |
| USB | Wireless USB bus |

### Cellular
A cellular network is a radio frequency distributed network that
divides geographic areas into cells. Cells are serviced by a fixed
location transceiver (base station).
* Cellular networks are used to transmit voice and data.
* Range is variable dependent upon the cell frequency.
* Cellular is a mature technology. Security controls have improved
with each generation; however, cellular networks are still
vulnerable to denial of service attacks.

### Cellular Tethering
Tethering is the connection of a device to a mobile device that has a means of accessing a network for the purpose of sharing the network access. Connecting a mobile phone to a laptop to charge the phone’s battery is not tethering. Connecting a mobile phone to a laptop so that the laptop can use the phone to connect to the Internet is tethering. When you tether a device, you create additional external network connections.

### Carrier Unlocking
Most mobile devices in the United States come locked to a carrier, while in other parts of the world they are unlocked, relying upon a subscriber identity module (SIM) for connection and billing information. This is a byproduct of the business market decisions made early in the mobile phone market lifecycle and has remained fairly true to date. If you have a carrier-locked device and you attempt to use a SIM from another carrier, the device will not accept it unless you unlock the device. Carrier unlocking is the process of programming the device to sever itself from the carrier. This is usually done through the inputting of a special key sequence that unlocks the device.

### The Global Positioning System (GPS)

GPS originally Navstar GPS, is a satellite-based radio navigation system owned by the United States government and operated by the United States Air Force. It is a global navigation satellite system that provides geolocation and time information to a GPS receiver anywhere on or near the Earth where there is an unobstructed line of sight to four or more GPS satellites. Obstacles such as mountains and buildings block the relatively weak GPS signals. GPS does not require the user to transmit any data, and it operates independently of any telephonic or internet reception, though these technologies can enhance the usefulness of the GPS positioning information. The GPS provides critical positioning capabilities to military, civil, and commercial users around the world. The United States government created the system, maintains it, and makes it freely accessible to anyone with a GPS receiver.

### GPS Tagging
Photos taken on mobile devices or with cameras that have GPS capabilities can have location information embedded in the digital photo. This is called GPS tagging by CompTIA, and geo-tagging by others. Posting photos with geo-tags embedded in them has its use, but it can also unexpectedly publish information that users may not want to share. For example, if you use your smartphone to take a photo of your car in the driveway and then post the photo on the Internet in an attempt to sell your car, if geo-tagging was enabled on the smartphone, the location of where the photo was taken is embedded as metadata in the digital photo. Such a posting could inadvertently expose where your home is located. There has been much public discussion on this topic, and geo-tagging can be disabled on most mobile devices. It is recommended that it be disabled unless you have a specific reason for having the location information embedded in the photo.


### Wi-Fi
Wi-Fi is a technology for wireless local area networking with devices
based on IEEE 802.11 standards
* Devices that can use Wi-Fi technology include personal computers,
video game consoles, smartphones, digital cameras, tablet
computers, smart TVs, digital audio players and modern printers.
* Wi-Fi compatible devices can connect to the Internet via a WLAN and
a wireless access point based on the IEEE 802.11 standards.
* Range depends on the frequency band, radio power output, antenna
gain, and antenna type as well as the modulation technique.
* Lessons 2.4 and 36.1 detail security concerns.

### Wi-Fi Direct/Ad Hoc
Wi-Fi typically connects a Wi-Fi device to a network via a wireless access point. Other methods exist, namely Wi-Fi direct and Wi-Fi ad hoc. In Wi-Fi direct, two Wi-Fi devices connect to each other via a single-hop connection. In essence, one of the two devices acts as an access point for the other device. The key element is the single-hop nature of a Wi-Fi direct connection. Wi-Fi direct connects only two devices, but these two devices can be connected with all of the bells and whistles of modern wireless networking, including WPA2. Wi-Fi direct uses a couple of services to establish secure connections between two devices. The first is Wi-Fi Direct Device and Service Discovery. This protocol provides a way for devices to discover each other based on the services they support before connecting. A device can see all compatible devices in the area and then narrow down the list to only devices that allow a specific service, say printing, before displaying to the user a list of available printers for pairing. The second protocol used is WPA2. This protocol is used to protect the connections and prevent unauthorized parties from pairing to Wi-Fi Direct devices, or intercepting communications from paired devices. The primary difference with Wi-Fi ad hoc is that in the ad hoc network, multiple devices can communicate with each other, with each device capable of communicating with all other devices.

### USB OTG
Universal Serial Bus is a common method of connecting mobile devices to computers and other host-based platforms. Connecting mobile devices directly to each other required changes to USB connections. Enter USB OTG (USB On-The-Go), an extension of USB technology that facilitates direct connection between USB OTG–enabled mobile devices. USB OTG allows those devices to switch back and forth between the roles of host and device, including deciding which provides power (host) and which consumes power across the interface. USB OTG also allows the connection of USB-based peripherals, such as keyboards, mice, and external storage, to mobile devices. Although USB OTG is relatively new, most mobile devices made since 2015 are USB OTG compatible.

### SATCOM
Satellite communications (SATCOM) systems relay and amplify
radio telecommunications signals via a transponder.
Communications satellites use an array of radio and microwave
frequencies.
* Communications satellites are used for television, telephone,
radio, Internet, and military applications.
* Security concerns include exploit of design flaws that can result
in injection, interception, and manipulation.

### Bluetooth
Bluetooth is a shortwave radio low power technology for
exchanging data based on the 802.15 standard. Originally
designed to replace RS-232 data cables.
* Bluetooth uses include headsets, hearing aids, wireless
speakers, PC input/out, health sensors, real-time location
systems, GPS receivers, bar coders, traffic control devices, and
game consoles.
* Range is 10-24m depending upon the version.

Subject to bluejacking and bluesnarfing:
* Bluejacking is injecting a unsolicited message.
* Bluesnarfing is unauthorized device access through a
Bluetooth discovery connection.

### Near field communication (NFC)
Near field communication (NFC) is a short range wireless
technology that requires close proximity and/or device contact.
NFC is rooted in RFID technology.
* NFC is used in commerce (e.g. contactless payment systems
such as Apple Pay), smartphone (sharing contacts, photos,
videos or files), identity and access tokens, and gaming.
* Range is less than 20 cm.
* Security concerns include eavesdropping, interception, and
theft.

##### Payment Methods
Twenty years ago, payment methods were cash, check, or charge. Today we have new intermediaries; smart devices with Near Field Communication (NFC) linked to credit cards offer a convenient alternative form of payment. While the actual payment is still a credit/debit card charge, the payment pathway is through the digital device. Utilizing the security features of the device, NFC, biometrics/pin, this form of payment has some advantages over the other methods as it allows additional specific security measures, such as biometric-based approval for the transaction, before accessing the payment method.

### ANT
ANT is a proprietary (but open access) multi-cast wireless sensor
network technology designed for the Internet of Things (iot).
* ANT is primarily incorporated into sports and fitness sensors
(wearables), though it may additionally be used for other
purposes.
* The transceivers/receivers are embedded in equipment such as
heart rate monitors, watches, cycling power meters, cadence
meters, and distance and speed monitors monitoring a user's
performance (e.g. Fitbit).
* Range is approximately 30 meters
* Security concerns eavesdropping, interception, impersonation.

### Infrared
Infrared (IR) is an optical (infrared light) shortwave
communication technology. IR is sometimes referred to as
beaming.
* IR is used in remote control devices, portable devices such as
mobile telephones, laptops, cameras, printers, and medical
devices.
* Range is <1m and requires line of sight.
* IR has been displaced by Wi-Fi and Bluetooth.

### Universal Serial bus (USB)
Wireless USB is a short—range, high—bandwidth radio bus
communication protocol.
* Wireless USB is used in game controllers, printers, scanners,
digital cameras, portable media players, hard disk drives, and
USB flash drives.
* Security concerns include packet loss and corruption.
* Range is 3-10 meters.
