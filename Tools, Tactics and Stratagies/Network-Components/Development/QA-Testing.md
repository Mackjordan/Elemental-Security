# Security Code Review
Security code review is the process of auditing the source code to verify that the proper security controls are present and work as intended.
* Static code analysis is the examination of non-running code (Static) for vulnerabilities.
* Dynamic analysis is the examination of running code for vulnerabilties.
https/www.cert.org/secure-coding/tools/index.cfm

### Static Code Analysis
Static analysis can be automated or manual. Manual code review is generally done by a peer developer; not the developer(s) who wrote the code. Advantages and disadvantages include:
* It can find weaknesses in the code at the exact location.
* Unique defects are detected that cannot or hardly be detected using dynamic tests.
* It must be conducted by trained software assurance developers who fully understand the code.
* It does not find vulnerabilities introduced in the runtime environment.

### Dynamic Analysis
Dynamic analysis is based the system execution. Dynamic testing is almost exclusively automated. Advantages and disadvantages include:
* Identifies vulnerabilties in the runtime environment
* Validates static code analysis findings
* Allows for analysis of applications in which you do not have access to the actual code
* Only as good as the tool used

### Software Quality Testing
Software quality testing focuses on the application in its entirety.
* Positive sting determines if the application works as expected
     * [Use Case] Test scenarios include load and volume system performance testing.
* Negative testing ensures that the application can gracefully and securely handle invalid input or unexpected behavior
     * [Misuse case] include populating required fields, input validation (including type of data, number of characters, data ranges), and system performance stress testing.

### System Performance Testing
##### Load Testing
* Load Testing Performance under normal and peak conditions.

##### Volume Testing
* Impact of incremental volume of records (not users).

##### Stress Testing
* Performance under an abnormal number of users or simultaneous operations.
