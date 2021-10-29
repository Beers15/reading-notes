
[Home](README.md)
 
# Readings: Authorization/Authentication

## Review, Research, and Discussion
 
---------------
 
1) What header(s) are used in authentication and authorization <sup>1</sup>
 
    Bearer, Basic, Hawk, API key (in request header), Digest, and AWS Signature, are some different variations of auth headers that are commonly used.
 
2) What is safe to put into a JWT
   
    Data that can be used to ID a user or any kind of security statement. This does not mean put a user's password in the payload of a JWT.
    
3) How are JWTs validated <sup>2</sup>

    Check that the JWT is well formed. Then check the signature. After this, check the standard claims. If all 3 of these steps pass, the token is validated. 

### Vocabulary terms
 
RBAC

  * Role Based Access Control: Actions a member of an application/organization/etc can make are based on their role. Different roles have different permissions.

User Roles

  * As touched on above, a role determines what a user can do. Generally speaking, the 'user' role has the most minimal subset of permissions compared to more advanced roles.

JWT Token

  * This stands for JSON Web Token. JWT is a standard for encoding data and exchanging it between 2 parties. Info about a user can be stored on the client side after being validated on the server using this standard.

### Preview

** No preparation materials were listed in today's reading assignment **
 
 
#### Works Cited

<sup>1</sup> Singh, Ankit, _Authorization header_, Async, Jun 19 2020, https://www.loginradius.com/blog/async/everything-you-want-to-know-about-authorization-headers/

<sup>2</sup>Auth0 Docs, _Validate JSON Web Tokens_, Auth0, Accessed Oct 28 2021, https://auth0.com/docs/security/tokens/json-web-tokens/validate-json-web-tokens