# What is OAuth

**What is OAuth?** OAuth is an open standard for access delegation, commonly used as a way for internet users to grant websites or applications access to their information on other websites but without giving them the passwords.

**Give an example of what using OAuth would look like.**  you can tell Facebook that it's OK for ESPN.com to access your profile or post updates to your timeline without having to give ESPN your Facebook password.

**How does OAuth work?** OAuth doesn't share password data but instead uses authorization tokens to prove an identity between consumers and service providers. OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password

**What are the steps that it takes to authenticate the user?** Identification. Users have to prove who they are.
Authentication. Users have to prove they are who they say they are.
Authorization. Users have to prove they're allowed to do what they are trying to do.

**What is OpenID?** OpenID is an open standard and decentralized authentication protocol promoted by the nonprofit OpenID Foundation

# Authorization and Authentication flows

**What is the difference between authorization and authentication?** 
Authentication and authorization are two vital information security processes that administrators use to protect systems and information. Authentication verifies the identity of a user or service, and authorization determines their access rights.

**What is Authorization Code Flow?** Authorization code flow is used to obtain an access token to authorize API requests. Authorization code flow is the most flexible of the three supported authorization flows and is the recommended method of obtaining an access token for the API.

**What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?** The Authorization Code Flow + PKCE is an OpenId Connect flow specifically designed to authenticate native or mobile application users. This flow is considered best practice when using Single Page Apps (SPA) or Mobile Apps. PKCE, pronounced “pixy” is an acronym for Proof Key for Code Exchange.

**What is Implicit Flow with Form Post?** Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.

**What is Client Credentials Flow?** In the client credentials flow, permissions are granted directly to the application itself by an administrator. When the app presents a token to a resource, the resource enforces that the app itself has authorization to perform an action since there is no user involved in the authentication.

**What is Device Authorization Flow?** With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text.

**What is Resource Owner Password Flow?** The Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token. This flow has significantly different security properties than the other OAuth flows.