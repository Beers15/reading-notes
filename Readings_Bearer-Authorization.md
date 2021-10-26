[Home](README.md)
 
# Readings: Bearer Authorization
 
## Review, Research, and Discussion
 
---------------
 
Referenced cited article below for answers<sup>1</sup>
 
1) (Correct?) order for questions 1 steps:

    Register your application to get a client_id and client_secret

    Ask the client if they want to sign in via a third party

    Redirect to a third party authentication endpoint

    Receive authorization code

    Make a request to the access token endpoint

    Receive access token

    Make a request to a third-party API endpoint

2) What can you do with an authorization code?

    This code can be used to obtain an access token and has a single use

3) What can you do with an access token?

    This token authorizes a user to perform actions that they have permission to take on a server, through an api endpoint

4) What’s a benefit of using OAuth instead of your own basic authentication?

    It's much more robust and secure than basic auth. It also allows the user to not provide sensitive information, such as a password.




### Vocabulary terms

Referenced cited article below for answers<sup>1, 2</sup>

Client ID

  * This is a public id for the app being used that is expected to be unique for every client of a specific auth server.

Client Secret

  * A value that only the app and the auth server have. It is used to prevent anyone from try to pass in to the server while pretending to be a certain client. It helps prevent the modification of JWTs.

Authentication Endpoint
  * The endpoint initially used by the user for them to verify their identity

Access Token Endpoint
  * This endpoint is used to exchange an authorization code. The code be be exchanged for an authorization code, which can be exchanged for an access token.

API Endpoint
  * The entry point/url for a service on a server. Endpoints are where the API can request resources from a server.

Authorization Code
  * This is a value used by an application to request an access token that is needed for authorizing certain actions.

Access Token
  * This token is used by an application to request data from an api. They are used to authorize certain tasks.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    How JWTs work

    The structure of JWTs and what each of the 3 parts(header, payload, and signature) is composed of

    What exactly a JWT token is in more detail    

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
 
    Specific use cases for when a JWT should be used

    Using the JWT library to actually implement the use of them in an application (both server side and client side)

    All the data flows and vocabulary of Auth0, 0Auth, and authorization+authentication in general.. It's still pretty confusing to fully comprehend at this time
 
3) What are you most excited about trying to implement or see how it works?
 
    Creating super secure services that handle auth tasks  
 
#### Works Cited
 
<sup>1</sup> Grimes, Roger and Fruhlinger, Josh, _What is OAuth? How the open authorization framework works_, CSO, Sep 20 2019, https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html

<sup>2</sup>Auth0, _Auth0 Docs_Accessed Oct 26 2021, https://auth0.com/docs/get-started