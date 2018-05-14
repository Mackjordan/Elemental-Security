# Identity Management Systems
Identity management (ldM) describes the management of user identities (including authentication and authorization) within and/or across enterprise boundaries.

Technologies include:
* Directory services
* Single sign-on
* Federated identity management

### Directory Services
A directory service is the centralized collection and distributed database (domain) of user data, computers, and trusted entities.

##### Directory services include:
* Lightweight Directory Access Protocol (LDAP).
* Microsoft Active Directory (AD) which is Microsoft’s implementation of LDAP.

##### LDAP attributes include:
* Scalability (billion + user entries).
* Distributable and synchronizable.
* Default LDAP port is 389, Secure LDAP is 636.

### Transitive Trust Relationship
If a user or application is authenticated by one domain, its authentication is accepted by all other domains that trust the authenticating domain.

* If a=b and b=c, then a=c.
* The effect of transitive trust in Windows domains is that there is complete trust between all domains in an Active Directory forest. Every domain has a transitive trust relationship with its parent domain, and every tree root domain has a transitive trust relationship with the forest root domain.

### Single sign-on (SS0)
SSO describes a unified login experience in which the user provides a set of credentials one time and is allowed to access multiple systems without needing to authenticate.
* SS0 system intercepts requests for identification and authentication.
* SS0 can be a bottleneck or single point of failure (SPOF).
* SSO rarely is a true enterprise solution and is often referred to as a legacy approach.

### Federated identity management (FIM)
FIM is an arrangement made among multiple enterprises that allows users to use the same identification data to obtain access to the networks of all enterprises in the group.
* Partners establish a mutual trust
* Identity is portable
