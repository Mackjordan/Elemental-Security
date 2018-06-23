# Federated Identity Management (FIM)
FIM is an arrangement made among multiple enterprises that allows users (and sometimes objects) to use the same identification data to obtain access to disparate resources.
* Technologies used for federated identity include Security Assertion Markup Language (SAML), OAuth, OpenID Connect, and Shibboleth.

### SAML Process
Security Assertion Markup Language (SAML) is an open standard that provides user authentication and authorization services.

##### SAML Components
* One-to-many model.
* End-user (Principal)
* Idenity Provider (IdP) = SAML-Compliant authentication service.]
* Service provider = SAML-Compliant web application.

### SAML Process
1. User (Principle) uses a web browser to access a web application and attempts to authentication.
2. The web application service provider (SP) requests an assertion from the identity Provider about the user.
3. The identity Provider (IdP) prompts the User for credentials (single or multi-factor)
4. User provides credentials.
5. If the User credentials are accepted, the Identity Provider (IdP) submits an assertion (Secure token) to the Service Provider (SP).
6. The Service Provider(SP) identifies the authorization level of the user and provides the appropriate level of access.

### Shibboleth
Shibboleth is a standards-based, open source software for web single sign—on across or within organizational boundaries.
* The Shibboleth software implements widely used federated identity standards, principally the SAML, to provide a federated
single sign-on and attribute exchange framework.
* Shibboleth also provides extended privacy functionality allowing a user and their home site to control the attributes released to each application.

### OAuth
OAuth 2.0 is an authorization framework that enables applications to obtain limited access to user accounts on an HTTP service such as Facebook or Twitter.

##### OAuth Components
* Resource Owner  
* Requesting Client
* Application
* Resource/Authorization Sewer API

### OAuth 2.0 Process
1. The application requests Authorization to access service resources from the User.
2. If the User authorizes the request, the Application receives an authorization.
3. The Application requests an access token from the authorization Server (API) by pressing its credentials and the user Authorization grant.
4. If the Application identity is accepted and the authorization grant is valid, the Authorization Server issues an Access Token to the Application.
5. The application presents the Access Token to the resource from the Resource server and requests access If Valid, the resource server serves the resource to the application.

### OpenID Connect
OpenID Connect is an identity layer on top of the OAuth 2.0 protocol which facilitates authentication.
* OpenlD connect verifies the identity of the end user.
* The id_token (secure token) includes information about the user.
* Can be used by both mobile and static applications.
