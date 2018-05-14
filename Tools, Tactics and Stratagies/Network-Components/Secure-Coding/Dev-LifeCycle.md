# Development Life Cycle

### Traditional Software Develoment
The traditional software development model is known as SDLC (system development |ifecycle)..s a linear (sequential) model.
* The Waterfall model requires that each phase must be completed before moving on to the next phase.
* The V-model emphasizes verification and validation at each phase and testing to take place throughout the project.

### Linear Models
##### Waterfall Model
1. Requirement
2. Design
3. Implementation
4. Verification
5. Maintenance

##### V-Model

   Requirements Analysis <---------------------------------> System Testing

         High Level Design <----------> Integration Testing

              Detailed Design <-----> Unit Testing
                            Implementation

### Evolutionary Models
Iterative and incremental project models develop software by using repeated cycles (iteration) related to specific functionality (Incremental).
* The Agile model uses iterative and incremental processes that emphasizes timebox team-based collaboration.
* Rapid application development (RAD) combines prototyping and iterative procedures.

### DevOps
The DevOps development methodology is built on the premise that collaboration between developers and the operations team is essential.
* The initial push for DevOps stemmed from the need to integrate operations to make software development more efficient and of higher quality.
* Integrated DevOps mandates that the operations team remains involved throughout the software development lifecycle to ensure a smooth, efficient process through transition and deployment.

### Secure DevOps
Instead of security continuing to exist as a standalone, isolated entity, secure DevOps aims to integrate security into the development processes from inception.
* The Secure DevOps approach enables developers to learn more about what they are developing and how it can be exploited.
* Secure DevOps proactively focuses on surviving by providing reliable software with a reduced attack surface.

### Including Security in the SDLC
“The inability to anticipate attacks is why we often see patches coming out in response to new zero-day vulnerabilities. Secure DevOps developers would rather their software absorb the attacks and continue to function.  In other words, it should bend but not break. This shift in thinking from a prevent to a bend-don’t-break mindset allows for a lot more flexibility when it comes to dealing with attacks. Ensuring a secure lifecycle requires the development team to focus on continuous integration, infrastructure as code, continuous deployment, and automated integrated development platform”

Hasan Yasar, https://insights.sei.cmu.edu/devops/2016/11/an-introduction-to-secure-devops-including-security-in-the-security-in-the-software-lifecycle.html

### Secure DevOps Concepts
##### Security Automation
* Automating attacks against pre-production code and continuous
vulnerability testing against production code

##### Continuous Integration (CI)
* CI is a continuous merging of source code updates from all developers on a team into a shared mainline. If a failure is seen, the development team is expected to refocus and fix the build before making any additional code changes

##### Baseline
* A consistent agreed upon version of software that serves as the basis
for further development.

##### Immutable Systems
* Image of a system preconfigured to a desired ”known good” state. Uses automation to replace rather than fix

##### Infrastructure as Code
* Using code to manage configurations and automate provisioning of
infrastructure (e.g. build testing and staging servers)

### The Future of Secure DevOps
Secure DevOps is a game changer.
* Developers at the frontline of security.
* Resilient applications and infrastructure.
* Automated, continuous, and integrated security testing.

### Supporting Processes
Three important internal processes support the current software development process:
* "Version control" tracks files, source code, and configurations over time.
* "Change control" manages changes to artifacts, such as code changes or documentation changes.
* "Provisioning" deploys (makes available) versions to various resources for simultaneous development.

### Version / Change Control Vocabulary. 

##### Baseline
* An approved revision of a document or source file from which subsequent changes can be made.

##### Tag
* User-friendly, meaningful name or revision number.

##### Check-out /co
* Create a local working copy from the repository

##### Diff/change/delta
* A specific modification to a document under version control

##### Commit
* Write or merge the changes made in the working copy back to the repository

##### Integration
* Two sets of changes are applied to a file

##### Changelog
* A record of all notable changes
