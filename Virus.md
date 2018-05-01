# Virus Overview
## A computer virus is a type of malware that, when executed, replicates itself by modifying other computer programs and inserting its own code. When this replication succeeds, the affected areas are then said to be "infected" with a computer virus. Malicious code whose primary function is to replicate and deliver its payload. 


Alt-H4


### Viruses come in a varity of forms.

Boot sector Virus: 
Infects the boot (First) sector of a drive. Loads into memory upon boot up. 

File Infector: 
Infects .com or exe files by overwriting original code. Can easily infect other executables with the same extension. 

Companion: 
Disguises itself as a legitimate program but uses a different extension with a higher priority. (Good.com to emulate good.exe)

Macro Virus: 
Written in a Macro language and is platform-independent. Infects and replicates templates and documents. 

Files types targeted include .bat, .com, .doc, .docx, dll, .exe, .html, .mdb, .pdf, .vbs, .xls, .xlsx, .zip. 



VirusTotal.com is online tool that aggregates many antivirus products and online scan engines to check for viruses that the user's own antivirus may have missed, or to verify against any false positives.Files up to 256 MB can be uploaded to the website or sent via email. Anti-virus software vendors can receive copies of files that were flagged by other scans but passed by their own engine, to help improve their software and, by extension, VirusTotal's own capability. Users can also scan suspect URLs and search through the VirusTotal dataset. 

You can add VirusTotal's functionality into your overall infrastructure using a script that can be automated to test resources againest VirusTotal’s database. 

Here’s an example. 
[https://github.com/Gawen/virustotal https://github.com/Gawen/virustotal]
