# Virus Overview

*A computer virus is a type of malware that, when executed, replicates itself by modifying other computer programs and inserting its own code. When this replication succeeds, the affected areas are then said to be "infected" with a computer virus. Malicious code whose primary function is to replicate and deliver its payload.*


## Viruses come in a variety of forms.

### Boot sector Virus:
*Infects the boot (First) sector of a drive. Loads into memory upon boot up.*

### File Infecter:
*Infects .com or .exe files by overwriting original code. Can easily infect other executables with the same extension.*

### Companion:
*Disguises itself as a legitimate program but uses a different extension with a higher priority. (Good.com to emulate good.exe)*

### Macro Virus:
*Written in a Macro language and is platform-independent. Infects and replicates templates and documents.*

### Files types targeted include:
*.bat, .com, .doc, .docx, dll, .exe, .html, .mdb, .pdf, .vbs, .xls, .xlsx, .zip.*

## Virus Characteristics.  

### Stealth Virus:
*Hides by encrypting its code. Masquerades as the original file and reports to that the original file intact.*

### Memory Resident:
*Upon execution stays resident in memory. Can infect other programs running at the same time.*

### Armored:
*Hides itself by obfuscation or by adding confusing or unnecessary code.*

### Polymorphic:
*Produces varied but operational copies of itself.*

### Metamorphic:
*Capable of recompiling itself into a new form.*

____
# Detection, Monitoring & Remediation

### Indicators of compromise (IOC):  

Indicators of compromise to a specific artifacts ( e.g. virus signature, IP address, Malicious URL, command & control connection, file changes. ) That with a high degree of confidence indicates an intrusion. Most malware will attempt to be covert and try to leave as few of artifacts as possible. Conversely, extortion attacks such as Ransomware and Adware are attention grabbing. 


### Antivirus (AV) software:

Antivirus software can be used to identify, contain, and in some cases eliminate known Malicious code. AV software relies on virus definition files (Known as DAT files) to identify malware. The definition files must be continually. Updated by the software publisher. Best Practices recommend using more than one type of AV in the enterprise.
Anti-malware software identifies infections caused by a pantheon of malware including viruses, worms, Trojan horses, rootkits, spyware, keyloggers, ransomware and adware.

[VirusTotal.com](https://VirusTotal.com) is online tool that aggregates many anti-virus products and online scan engines to check for viruses that the user's own anti-virus may have missed, or to verify against any false positives.Files up to 256 MB can be uploaded to the website or sent via email. Anti-virus software vendors can receive copies of files that were flagged by other scans but passed by their own engine, to help improve their software and, by extension, VirusTotal's own capability. Users can also scan suspect URLs and search through the VirusTotal dataset.

> #### You can add VirusTotal's functionality into your overall infrastructure using a script that can be automated to test resources against VirusTotal’s database. Here’s an example of a script that can be used to automate the process of searching your files using VirusTotal.com. It's written in Python and  
> #### [Gawen/virustotal](https://github.com/Gawen/virustotal)
