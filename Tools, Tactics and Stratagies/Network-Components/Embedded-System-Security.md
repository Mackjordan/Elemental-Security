# Embedded System Defined
An embedded system is an electronic product that contains a microprocessor and software designed to perform a specific task. An embedded system can either be fixed or programmable.
* Embedded systems are found in consumer, cooking, industrial, automotive, medical, commercial, and military applications.
* Embedded systems range from very small personal devices to large-scale environments. For example, digital watches, health meters, printers/MFDs, camera systems, routers, sensor traffic lights, automotive safety, and industrial control systems.

### Embedded System Components.
An embedded system generally has three ”closed loop" components.
1. System on a chip (SoC) which is microprocessor or microcontroller with advanced peripherals such as Wi-Fi.
2. Real-time Operating System (RTOS) that defines the way the system works.
3. Application software specific to the device.


### Vulnerabilities
Why are embedded devices vulnerable?
* Devices are designed for functionality and convenience — not security.
* Devices are powered by specialized computer chips/RTOS. The chips are inexpensive and profit margins slim. Strong incentive to use open source operating systems and components. Often the software is outdated.
* Little incentive to maintain chips/RTOS. Often, patches are not available. If available, expertise to install is rare or the incentive nil.

### Embedded System Attacks
##### Network Attack
Exploit the protocol or implementation (e.g. open ports)
* Injection (e.g. persistent malware)
* Privilege escalation
* Packet capture

##### Active Side Channel
* Using a voltage glitch on the power supply to cause a program malfunction.

##### Memory and Bus
* Physically connect to the hardware and read the contents of the memory.

##### Weak Authentication
* Using the known default administrator password to gain access.

##### Botnet
* Weaponization of devices (botnets) for use in DDoS attacks

##### Stepping Stone
* Embedded devices such as HVAC systems, printers/MFDs, and camera systems are often connected to a network unmanaged

### ICS / SCADA
Industrial Control Systems (ICS) are embedded systems that monitor and control industrial processes that exist in the physical world. ICS are either data—driven or operated remotely.
* SCADA usually refers to centralized systems which monitor and control entire sites, or complexes of systems spread out over large areas (e.g. electricity, natural gas, gasoline, water, waste. treatment, transportation).
* Top threats include cyberattack by politically motivated adversaries and human error.
* Top challenges include lack of or weak authentication mechanisms, minimal visibility, outdated operating systems, and inability to patch.

### Increasingly Serious Issue
Embedded systems are pervasive and the ease of exploit appears to be increasing. The Internet of Things (loT) sensors and actuators embedded in physical objects—from roadways to pacemakers—are linked through wired and wireless networks
provide a pathway for attack.
* Wearable technology
* Home automation
* Medical Devices
* Vehicles and Aircraft

### Best practices for evaluating and securing embedded devices
include:
* Research supply chain including chip manufacturer and software
* Research available security controls before purchasing
* Immediately change the default credentials
* Use strong and unique passwords (multi-factor, if available)
* Disable features and services that are not required
* Disable Telnet login and use SSH where possible
* Segregate embedded devices whenever possible
* Disable or protect remote access to devices when not needed
* Regularly check the manufacturer’s website for firmware updates
