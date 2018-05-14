# Secure Staging
Secure staging is the process planning, scheduling, and controlling the movement of developed or acquired code.
* The primary goal is to protect the integrity of the ”live” production environment and ensure that security baselines are met.
* Security baselines are standards that reflect the minimum requirements necessary to avoid putting a network at risk.
* Environment, in the context of secure staging, refers to the host device (physical or virtual) including connectivity.
* A sandbox is an isolated environment. The most common configuration is running an application is a restricted ' memory area.

### Secure Staging Workflow

1. DEV
2. TEST
3. STAGE
4. PROD

### Integrity Measurement
Best case scenario is for developers to identify bugs and issues during the development state. Early identification is more efficient and less expensive.
* Integrity measurement is a measure of the quality of the source code before it moves to the test environment.
* Unit testing evaluates a module for specification compliance (including security baseline).
* Interface testing evaluates the connection between two or more components.

### TEST
The testing environment (TEST) is used to merge code, ensure quality, isolate bugs, and measure performance and functionality. Testing and development are iterative processes.
* The testing environment should match the production environment as closely as possible.
* User acceptance testing (UAT) can be multi-stage.
* Alpha versions are early versions submitted for feature and functionality testing and feedback.
* Beta versions are late stage versions submitted to a limited set of users for testing and feedback.
* The testing environment MUST be segregated from the production environment.

### STAGE (AKA Pre-PROD)
The staging environment (STAGE) is used to ensure that the application behaves as expected and confirms that it does not adversely impacting existing applications.
* The staging environment should mirror the production environment.
* No actual code development should ever take place on a staging server (no developer permissions).
* Security testing should always take place at this stage.
* Rollback procedures should be tested.
* Management approval (sign-off) should be given before an application moves into production.

### PROD
The production environment (PROD) is the ”live” environment that hosts the application. It is the endpoint in the release management process.
* PROD planning should include deployment, maintenance, backup, and disaster recovery strategies.
* Developers should never have rights to a PROD environment (segregation of duties).
* New functionality and bug fixes should go through the release management cycle before being deployed to PROD.
* Emergency changes should be subject to change management procedures.
