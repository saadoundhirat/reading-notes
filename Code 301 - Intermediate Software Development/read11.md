## Readings: Authentication

# **What is auth**

----------

## **What is OAuth?**

* **Answer:**

* OAuth allows websites and services to share assets among users. It is widely accepted.
* OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization

## **Give an example of what using OAuth would look like?**

* **Answer:** OAuth scenario could be a user sending cloud-stored files to another user via email, when the cloud storage and email systems are otherwise unrelated other than supporting the OAuth framework (e.g., Google Gmail and Microsoft OneDrive). When the end-user attaches the files to their email and browses to select the files to attach, OAuth could be used behind the scenes to allow the email system to seamlessly authenticate and browse to the protected files without requiring a second logon to the file storage system.

## **How does OAuth work? What are the steps that it takes to authenticate the user?**

* **Answer:** Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified):

1- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

2- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

3- The first site gives this token and secret to the initiating user’s client software.
The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

4- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

5- The user approves (or their software silently approves) a particular transaction type at the first website.

6- The user is given an approved access token (notice it’s no longer a request token).

7- The user gives the approved access token to the first website.

8- The first website gives the access token to the second website as proof of authentication on behalf of the user.

9- The second website lets the first website access their site on behalf of the user.

10- The user sees a successfully completed transaction occurring.

11- OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

## **What is OpenID?**

* **Answer:**  "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."

---------

# **Authorization and Authentication flows**

## **What is the difference between authorization and authentication?**

* **Answer:**In authentication process, the identity of users are checked for providing the access to the system. While in authorization process, person’s or user’s authorities are checked for accessing the resources. Authentication is done before the authorization process, whereas authorization process is done after the authentication process.


![Authentication and Authorization](https://media.geeksforgeeks.org/wp-content/uploads/20190606141632/Untitled-Diagram-2019-06-06T141540.818.png)

## **What is Authorization Code Flow?**

* **Answer:** Authorization code flow is used to obtain an access token to authorize API requests. ... Access tokens, obtained using authorization code flow, provide permissions for your application to manipulate documents and other resources on behalf of a Mendeley user and make requests for all API resources.

## **What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

* **Answer:** The Authorization Code Flow + PKCE is an OpenId Connect flow specifically designed to authenticate native or mobile application users. This flow is considered best practice when using Single Page Apps (SPA) or Mobile Apps. PKCE, pronounced “pixy” is an acronym for Proof Key for Code Exchange.

## **What is Implicit Flow with Form Post?**

* **Answer:** Implicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. The web app requests and obtains tokens through the front channel, without the need for secrets or extra backend calls.

## **what is client credentials flow?**

* **Answer:** The Client Credentials flow is a server to server flow. There is no user authentication involved in the process. ... Since there is no user authorization, the flow only interacts with the Token endpoint.

![client credentials flow](https://developer.ebay.com/api-docs/res/resources/images/ebay-rest/client_credentials_650x449.png)

## **What is Device Authorization Flow?**

* **Answer:** The OAuth 2.0 Device Authorization Grant (formerly known as the Device Flow) is an OAuth 2.0 extension that enables devices with no browser or limited input capability to obtain an access token. This is commonly seen on Apple TV apps, or devices like hardware encoders that can stream video to a YouTube channel.

## **What is Resource Owner Password Flow?**

* **Answer:** The Resource Owner Password Credentials flow allows exchanging the username and password of a user for an access token and, optionally, a refresh token. The primary difference is that the user's password is accessible to the application. ...

![Resource Owner Password Flow](https://www.oreilly.com/library/view/getting-started-with/9781449317843/httpatomoreillycomsourceoreillyimages986441.png)

------

### **resources**

recource      | links
------------- | -------------
What is OAuth  | [Link](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)
What is Authorization Code Flow | [Link](https://dev.mendeley.com/reference/topics/authorization_auth_code.html#:~:text=Authorization%20code%20flow%20is%20used,token%20to%20authorize%20API%20requests.&text=Access%20tokens%2C%20obtained%20using%20authorization,requests%20for%20all%20API%20resources.)
Auth Code Flow + PKCE
 | [Link](https://developers.onelogin.com/openid-connect/guides/auth-flow-pkce#:~:text=The%20Authorization%20Code%20Flow%20%2B%20PKCE,Proof%20Key%20for%20Code%20Exchange.)
Authentication and Authorization Flows | [Link](https://auth0.com/docs/flows)
