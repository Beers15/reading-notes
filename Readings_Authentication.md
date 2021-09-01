[Home](README.md)

# Readings: Authentication

### What is OAuth
---------------

Referenced the source below for answers<sup>1<sup>

1. What is OAuth?
  "OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential."<sup>1<sup>

2. Give an example of what using OAuth would look like.
  A website allows you to log in to their site with another service's login. (e.g. Google's, FB's, etc authenticate options on many sites).

3. How does OAuth work? What are the steps that it takes to authenticate the user?
  * 1st site connects to 2nd site with OAuth with a verified user ID.
  *  2nd site makes a 1-time token. The 1st time takes this token, and a 'secret' and gives it to the initiating client's software. 
  * Client software sends token to authorization provider and will have to authenticate said provider if they've not done so yet.
  *  User approves of their transaction on the 1st site and then recieves a approved access token which they send to the 1st site.
  *  The 1st site then sends the access token to the 2nd site and this serves as proof of authentication. 
  * The 2nd site allows 1st site access now. 
  * The user can see the completing transaction happening.

4. What is OpenID?
  OpenId os conserned with authentication of a user rather then the authorization of a transaction. It is used to vouch for the ID of users.

### Authorization and Authentication flows
---------------

Referenced the source below for answers<sup>2<sup>

1. What is the difference between authorization and authentication?
  *Authorization: ensure user has permission to perform a certain task
  *Authentication: ensure user is who they say they are

2. What is Authorization Code Flow?
  * User hits login and AUTH0's SDK does a redrect to Auth0 auth server
  * The Auth0 auth server redirects user to login + auth prompt
  * User is presented with login options and chooses one
  * A Auth server redirects back to app with a 1 use token
  * Auth0's SDK sends token to its /oauth/token endpoint and also sends the ID and client 'secret'
  * Auth0 auth server then sends a response with the ID Token, Access Token, and sometimes a refresh token.
  * Original app can use this access token to call an API and get info about user
  * Finally, the API responds with the data that the user requested

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

  This is similar to the above control flow. The main difference is that there is a cryptographically-random  code_verify value generated along with a 'code_challenge' and this code_challenge is used instead of a access token. After following similar steps, the AUth0 auth server verifies these 2 values before providing the same tokens back to the Auth0 SDK. This also results in the API responding with the requested data.

4. What is Implicit Flow with Form Post?
  * User hits login in an app
  * Auth0's SDK redirects the user to its /authorize endpoint and passes to it response_type, id_token, and response_mode param of form_post
  * User chooses one of the provided login options and then sees a list of permissions Auth0 will give to the app
  *Auth0 auth server redirects user back to the original app with an ID token.

5. What is Client Credentials Flow?
  * An app authenticates itself with Auth0 auth server with the client ID and client secret at the /oauth/token endpoint
  * The Auth0 auth server validates these 2 values and responds with an access token
  *  The app uses this token to call the related API and then the API responds with requested data

6. What is Device Authorization Flow?
The user starts the app on the device.

  * An app on a device requests authorization from the Auth0 auth server from the /oauth/device/code endpoint and provdes a client id.

  * Auth0 auth server then sends  a device_code, user_code, verification_uri, verification_uri_complete expires_in, and polling interval back to the app.

  * The app on the device being used asks user to activate using a computer or smartphone. This can be done with a QR code, visting a specfic uri and entering a code, or navigating to a verification page with the embedded verification_uri_complete value.

  * The app on the device polls to recieve an access token from the Auth0 auth server for an Access Token at the /oauth/token endpoint. The device app will poll until either the browser flow path or the user code expires user completes.
z
* When the user successfully completes the browser flow path, your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token). The device app should now forget its device_code because it will expire.

Your device app can use the Access Token to call an API to access information about the user.

The API responds with requested data.

Browser Flow


7. What is Resource Owner Password Flow?

## Things I want to know more about
---------------
* How to implement these control flows using the Auth0 React SDK


###### Works Cited

<sup>1</sup> Grimes, Rpger _What is OAuth? How the open authorization framework works_, CSO, Sep 20 2019, https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html

<sup>2</sup> Auth0 Docs _Authentication and Authorization Flows_, Auth0, Accessed 8/31/2021, https://auth0.com/docs/authorization/flows