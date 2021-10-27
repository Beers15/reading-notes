[Home](README.md)
 
# Readings: Access Control (ACL)
 
## Review, Research, and Discussion
 
---------------

1) When is Basic Authorization used vs. Bearer Authorization?<sup>1</sup>

    Basic Authorization is when the client needs to authenticate itself with username and password. It is useful in situations were not having cookies, sessions or login pages is preferred. Bearer auth is commonly used for OAuth, OAuth2. Bearer auth is useful because it doesn't require anything to be stored on the server in regards to each specific user since the JWT has the user data embedded in it.

2) What does the JSON Web Token package do?

    It is used to create, verify, and configure JWTs.

3) What considerations should we make when creating and storing a SECRET?

    You want to make your SECRET completely unguessable and only share it with people within a project that you trust. Store using a secure medium either physically or online, or both.

### Vocabulary terms

Referenced cited article below for answers<sup>1, 2</sup>

encryption<sup>2<sup>

  * This is the process of encoding data. The original data, or 'plaintext' is converted into ciphertext

token

  * Tokens are pieces of data passed during the auth process that represent a user, a set of permissions, or some other relevant information in the auth process.

bearer<sup>3</sup>

  * This is a type of authorization that involves using token authentication. A  token is encrypted into a string that is passed along with in the header of a request to an App's server. The bearer of a signed token is then granted certain permissions.

secret

  * A secret is some value that is used to sign tokens. When coupled with certain libraries, this makes incoming tokens to a server checkable for tampering. Even with an intercepted token, someone can't mimic what the server is expected without the correct secret. 

JSON Web Token

  This is a standard for sending data in a secure manner. It is used with the OAuth protocol in authorization control flows.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    ACLs in Linux

    The concepts of ABAC and RBAC outside of a programming context

    Steps to take when implementing a RBAC system

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    How to implement RBAC in an authorization server
 
    What the benefits of RBAC when it comes to authorization 

    When to use RBAC vs ABAC vs ACL 
 
3) What are you most excited about trying to implement or see how it works?
 
    Implementing role based access control in an authorization server 
 
#### Works Cited
 
<sup>1</sup> DaNeil, _So Many Auths!_, DEV, Aug 12 2019, https://dev.to/caffiendkitten/authentication-types-3984

<sup>2</sup>Wikipedia, _Encryption_, Accessed Oct 27 2021, https://en.wikipedia.org/wiki/Encryption

<sup>3</sup>Swagger, _Bearer Authentication_, Accessed Oct 27 2021, https://swagger.io/docs/specification/authentication/bearer-authentication/