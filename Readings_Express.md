[Home](README.md)

# Readings: Express

## Review, Research, and Discussion

---------------

1) What’s the difference between PUT and PATCH?

    PUT is a complete update of a resource, it replaces a resource with a full resource. Whereas PATCH is a partial update of a resource. PATCH changes parts oof the resource and modifies some properties, but the updated resource at the location is the same before and after.<sup>1</sup>

2) Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

    Beeceptor https://beeceptor.com/

    MockServer https://www.mock-server.com/

    WireMock http://wiremock.org/

3) Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

    An api that incorporates swagger can have interactive documentation automatically generated when the application is configured properly. Documentation can be yml or JSON. It also supports automated testing. Swagger is more widely used than APIDOC.

    APIDOC also generates documentation for source code. It documents files as multiline comments with @annotations and has a command line interface.<sup>2</sup>

    4xx and 5xx series status codes should be sent for unsuccessful API calls. 3xx status codes may also be sent if additional actions are needed for a request (request in this state is not necessarily a success yet).

4) Compare and contrast SOAP (Simple Object Access Protocol and Representational State Transfer) and ReST

    Both SOAP and ReST are alike in the following ways:
    They both work with XML format. A web service can use either one for an API. They are both techniques used for developing various web services.

    Here are some ways in which they differ:
    SOAP is a protocol and ReST is an architectural style.
    SOAP is generally considered better for security and addressing, and ReST is considered better for CRUD operations on resources.
    SOAP is limited to XML format. ReST can format data using plain text, HTML, JSON, and more.
    There are various instances where one technique may be better to use the other when developing a web service (some instances can be found in the cited article below)<sup>3</sup>

### Vocabulary terms

* Web Server
This refers to the software and/or hardware that handles incoming requests made by clients. It can store and serve various files that make up a website and can use HTTP to deliver those resources to users based on a supplied url.<sup>4</sup>

* Express
Express is a minimalist, unopinionated web framework that is used for creating servers, handling incoming http requests, working with a rendering engine to serve views, defining + using middleware, configuring a multitude of settings for the created servers, and much more.<sup>5</sup>

* Routing
Routing is the actions a web server takes when a user makes a request to a certain endpoint that that server is configured to handle. Express defines a route by specifying the HTTP Method, uri, and a route handler method to execute when that uri is hit on the related server/routing object. Defines the uri and actions to take here is a form of routing.

* WRRC
This stands for the Web Request Response cycle. A client makes a HTTP request to a server that uses one of the HTTP methods. THe server processes that request and sends a response back.


### Things I want to know more about

---------------

<<<<<<< HEAD
#### Works Cited

<sup>1</sup>Ola, Segun, _RESTful API Design — PUT vs PATCH_, Segunolalive, Mar 13 2018, https://blog.segunolalive.com/posts/restful-api-design-%E2%80%94-put-vs-patch/

<sup>2</sup>asptricks.net, _apidoc vs swagger for node app_, https://www.asptricks.net/2019/04/apidoc-vs-swagger-for-node-app.html

<sup>3</sup>Walker, Alyssa, _SOAP Vs. REST: Difference between Web API Services_, Guru99, Oct 8 2021, https://www.guru99.com/comparison-between-web-services.html

<sup>4</sup>MDN, _What is a web server?_, https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server

<sup>5</sup>MDN, _Express/Node introduction_, https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction

[Home](README.md)

# Readings: Express

## Review, Research, and Discussion

---------------

1) What’s the difference between PUT and PATCH?

    PUT is a complete update of a resource, it replaces a resource with a full resource. Whereas PATCH is a partial update of a resource. PATCH changes parts oof the resource and modifies some properties, but the updated resource at the location is the same before and after.<sup>1</sup>

2) Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

    Beeceptor https://beeceptor.com/

    MockServer https://www.mock-server.com/

    WireMock http://wiremock.org/

3) Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

    An api that incorporates swagger can have interactive documentation automatically generated when the application is configured properly. Documentation can be yml or JSON. It also supports automated testing. Swagger is more widely used than APIDOC.

    APIDOC also generates documentation for source code. It documents files as multiline comments with @annotations and has a command line interface.<sup>2</sup>

    4xx and 5xx series status codes should be sent for unsuccessful API calls. 3xx status codes may also be sent if additional actions are needed for a request (request in this state is not necessarily a success yet).

4) Compare and contrast SOAP (Simple Object Access Protocol and Representational State Transfer) and ReST

    Both SOAP and ReST are alike in the following ways:
    They both work with XML format. A web service can use either one for an API. They are both techniques used for developing various web services.

    Here are some ways in which they differ:
    SOAP is a protocol and ReST is an architectural style.
    SOAP is generally considered better for security and addressing, and ReST is considered better for CRUD operations on resources.
    SOAP is limited to XML format. ReST can format data using plain text, HTML, JSON, and more.
    There are various instances where one technique may be better to use the other when developing a web service (some instances can be found in the cited article below)<sup>3</sup>

### Vocabulary terms

* Web Server
This refers to the software and/or hardware that handles incoming requests made by clients. It can store and serve various files that make up a website and can use HTTP to deliver those resources to users based on a supplied url.<sup>4</sup>

* Express
Express is a minimalist, unopinionated web framework that is used for creating servers, handling incoming http requests, working with a rendering engine to serve views, defining + using middleware, configuring a multitude of settings for the created servers, and much more.<sup>5</sup>

* Routing
Routing is the actions a web server takes when a user makes a request to a certain endpoint that that server is configured to handle. Express defines a route by specifying the HTTP Method, uri, and a route handler method to execute when that uri is hit on the related server/routing object. Defines the uri and actions to take here is a form of routing.

* WRRC
This stands for the Web Request Response cycle. A client makes a HTTP request to a server that uses one of the HTTP methods. THe server processes that request and sends a response back.


### Preview


1) Which 3 things had you heard about previously and now have better clarity on?

  Express, TDD, and route handlers

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

  Mocking apis in order to test them, unit testing, and publishing to NPM

3) What are you most excited about trying to implement or see how it works?

  Going more in depth with jest for TDD and configuring tests for continuous integration.

### Things I want to know more about

---------------

=======
>>>>>>> 496a0fe68001254e34f118fd854157c5733456cd
* How to develop an API using the SOAP protocol.

* How to utilize mock API tools and documentation generation tools+services like apiDoc and Swagger when building a web application.

#### Works Cited

<sup>1</sup>Ola, Segun, _RESTful API Design — PUT vs PATCH_, Segunolalive, Mar 13 2018, https://blog.segunolalive.com/posts/restful-api-design-%E2%80%94-put-vs-patch/

<sup>2</sup>asptricks.net, _apidoc vs swagger for node app_, https://www.asptricks.net/2019/04/apidoc-vs-swagger-for-node-app.html

<sup>3</sup>Walker, Alyssa, _SOAP Vs. REST: Difference between Web API Services_, Guru99, Oct 8 2021, https://www.guru99.com/comparison-between-web-services.html

<sup>4</sup>MDN, _What is a web server?_, https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server

<sup>5</sup>MDN, _Express/Node introduction_, https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction
