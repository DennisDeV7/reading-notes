# Authentication

## OAuth

1. What is OAuth?\
OAuth is a secure, third party, user-agent delegated authorization.
2. Give an example of what using OAuth would look like.\
An example of OAuth is a login screen that offers to log on using another website's logon
3. How does OAuth work? What are the steps that it takes to authenticate the user?\
    1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
    2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
    3. The first site gives this token and secret to the initiating user’s client software.
    4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    6. The user approves (or their software silently approves) a particular transaction type at the first website.
    7. The user is given an approved access token (notice it’s no longer a request token).
    8. The user gives the approved access token to the first website.
    9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
    10. The second website lets the first website access their site on behalf of the user.
    11. The user sees a successfully completed transaction occurring.
    12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).
4. What is OpenID?
OpenID is a security technology similar to OAuth except it is for humans to log onto machines instead of machines loggin into machines.

## Authoraization and Authentication Flows

1. What is the difference between authorization and authentication?\
Authentication is the process of verifying who a user is. Authorization is the process of verifying what the user has access to.
2. What is Authorization Code Flow?\
Authorization Code Flow exchanges an authorization code for a token.
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?\
PKCE has the calling application create a secret that can be verified by the authorization server.
4. What is Implicit Flow with Form Post?\
Implicit Flow with Form Post requests and obtains tokend thorugh the front channel, without the need for secret backend calls
5. What is Client Credentials Flow?\
Client Credentials Flow authorizes an app rather than a user
6. What is Device Authorization Flow?\
In Device Authorization Flow, the device will ask the user to go to a link that will authorize the device
7. What is Resource Owner Password Flow?\
Resource Owner Password Flow asks for credentials (username, password) by using a form

## Class

## Things I want to know more about
