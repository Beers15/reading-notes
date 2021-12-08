[Home](README.md)
 
# Readings: API Integration
 
## Review, Research, and Discussion
 
---------------
All answers taken from the resources below

1) How do bearer tokens work?

  * A bearer token is an encrypted string that contains a payload and information about a user, or the 'bearer' of the token. It is sent as part of the HTTP "Authorization" header and used to authenticate an API request. In the OAuth framework, this token is used to obtain an access token.

2) Describe express middleware

  * Express middleware are functions that run on an express app between the initial request and the final response while having access to the request object. They are chained and can be configured to only run on certain routes.

3) What is a JWT?

  * JWT is a standard for transferring data securely between 2 parties. This data can be signed with a 'secret' value before being sent and then verified on the other side using the same 'secret' value. JWT is commonly used for authorization.

### Vocabulary terms

role based access control

  * This is a security approach where certain actions are only able to be performed by entities with the proper role. Roles contain various capabilities which define what someone of that role can do.

http cookies

  * These are bits of data that are send both to and from a server using HTTP that is stored in a user's browser. They usually store some bit of data related to a user's session.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?

    * JWTs
    * bearer authorization 
    * Using authorization related express middleware

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * How to better use JWTs to handle authorization and send data securely  
    * How to make better use of RBAC in an app 
    * Using HTTP cookies
 
3) What are you most excited about trying to implement or see how it works?
 
    * I've integrated APIs into my front-ends that implemented auth before. I want to learn how that works in depth since I didn't have good grasp on authorization tasks where the functionality was largely provided by 3rd party libraries. 

--------------

### Resources

https://developer.okta.com/blog/2018/09/13/build-and-understand-express-middleware-through-examples

https://www.oauth.com/oauth2-servers/differences-between-oauth-1-2/bearer-tokens/

https://jwt.io/introduction