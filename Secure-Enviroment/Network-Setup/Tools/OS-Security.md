# Operating Systems
The function of an operating system is threefold: manage resources, execute services and applications, and establish a user interface.
* A trusted operating system is one that supports multilevel security and meets a specific set of government requirements.
* A trusted operating system must meet two criteria:
    1. Enforcement of a security policy
    2. Sufficient measures of assurance

### OS types.
| Type | Description |
|------|-------------|
| Network | A network OS has special functions for connecting devices. Generally, a network OS is embedded in a device (e.g. router).|
| Server | A server OS is designed to centralize functions (e.g. authentication, DHCP, DNS) and applications, share resources , and manage multiple concurrent client requests. |
| Workstation | A workstation OS is primarily designed to run applications for a logged in user. |
| Appliance | Just Enough Operating Systems (JeOS - pronounced ’juice’) is a minimal (JeOS) customized OS to fit the need of a specific appliance. |
| Kiosk | A kiosk OS is a minimal ”locked down" OS that generally defaults to original state at the end of a session. |
| Mobile | A mobile 05 is lightweight and specifically designed for mobile devices. Mobile OSs are generally device specific.|

### Hardening an operating System
Hardening an operating system is the process of configuring security settings, rules, and policies and removing unnecessary applications and services in order to minimize vulnerabilities and exposure to threats.
* A security baseline is a set minimum requirements for hardening a system.

### Applying Patches and Hot Fixes
Operating system vulnerabilities are continually being identified. Publishers release code patches designed to fix or mitigate vulnerability.
* Unless there is a compelling reason not to, operating systems should always have the latest updates installed.
* Windows SystemInfo command will display patches.
* Patch management is the on-going process of planning, testing, deploying, and auditing patches.

### Least Functionality
The NIST SP800-53 configuration management principle of least functionality states that ”information systems should be configured to provide only essential capabilities and specifically prohibit or restrict the use of functions, ports, protocols, and
services”.

In practice this means:
* Testing and auditing the system for compliance.
* Deleting unused programs.
* Disabling services.

### Disabling Services
A service is an application that runs in the background. Disabling unnecessary service minimizes exposure and enhances performance.
* A service can be configured to start automatically at boot-up.
* A service is independent of the logged in user and will continue to run even if there are no logged in users.
* Services typically run in the context of the Local System Account (administrative privileges).

### Removing Unused Programs
Every application has potential vulnerabilities. Applications advertise via listening ports. If the application is not being used, uninstalling it reduces the potential attack surface.
* Make sure to remove all components and earlier versions.
* If an application is required, ensure that is it included in a patch management and application update program.

### Black and White listing
In an enterprise environment, security policies can be used to control application access.
* An application white listing policy allows only applications that are explicitly given permission to run on a client computer. All other applications are denied
* An application blacklisting policy allows all applications to run on a client computer with the exception of those that are explicitly denied.

### Disabling Default Accounts
Default accounts are accounts that are created by the operating system or application. Depending upon the environment, some of these user and group IDs can become security weaknesses, vulnerable to exploitation.
* Review default account (e.g. admin, guest, SA, service accounts).
* If the account is required, create an account with equivalent privileges and disable the original account. If it is not possible to create an equivalent account, then rename the original and change the default password.
* If the account is not required, disable (delete if possible) the account.

### Windows AD Group Policy
Group Policy provides centralized management and configuration of operating systems, applications, and users' settings in an Active Directory environment.

### Peripheral Security
Wireless keyboards and mice, displays, Wi-Fi-enabled microSD cards, printers, multifunction devices, external storage devices, digital cameras, and other peripherals all are potentially vulnerable and subject to exploit.
Best practices to minimize threats include:
* Reject ”unknown” devices (disallow using policies)
* Change the default password .
* Use secure connectivity protocols (e.g. SSH instead of Telnet)
* Disable unnecessary services (e.g. remote management)
* Configure access controls
* If applicable, use secure wireless protocols
* Dispose of securely
