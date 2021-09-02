[Home](README.md)

# Readings: CRUD

### Status Codes Based On REST Methods
---------------

Referenced the source below for answers<sup>1<sup>

1. In your own words, describe what each group of status code represents:

  100’s = This series of codes signifies that an informational response will be sent and that the server will try to send back what was requested
        
  200’s = This series signifies various types of successful requests.
        
  300’s = This series signifies types of redirection. The resource isn't available at the location the user requested it from.
  
  400’s = This series signifies way a request failed.
  
  500’s = Similar to the 400's series, but for server related errors.

2. What is a status code 202?

  The resource was properly validated when it was sent, but not that the request has been completed. It is used with asynchronous requests.

3. What is a status code 308?

  This code lets the client know the the resource is not avaiable at the chosen url, but provides another url where it is available.

4. What code would you use if an update didn’t return data to a client?

  I'd probably use a 404 code, since the resource was not found.

5. What code would you use if a resource used to exist but no longer does?

  You would use a 410 status code.

6. What is the ‘Forbidden’ status code?

  The 403 status code is the 'Forbidden' status code.


### Build A REST API With Node.js, Express, & MongoDB - Quick
---------------

Referenced the source below for answers<sup>2<sup>

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?
  To keep it from showing in our source code and maintain database security.


2. What is middleware?

  Middleware that is run after the request and before the response.

3. What does app.use(express.json()) do?

  This lets server accept json as part of the body of a request. This is especilly useful for PUT and POSTS requests.

4. What does the /:id mean in a route?

  That means that there is a route parameter which is at the end of a supplied uri with the name of id.

5. What is the difference beween PUT and PATCH?

  PUT creates or wholly updates a resource. PATCH does a partial update of the resource.

6. How do you make a default value in a schema?

7. What does a 500 error status code mean?

  This is a generic error response status code for a server related issue.

8. What is the difference between a status 200 and a status 201?

  Both codes mean successful request was made, but the 201 also means that a new resource was created.


## Things I want to know more about
---------------
* Defining custom middleware functions


###### Works Cited

<sup>1</sup> Kay Ploesser, _Which HTTP Status Code to Use for Every CRUD App _, API Product Management, moesif Blog, Apr 16 2020, https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/understanding-the-javascript-call-stack-861e41ae61d4/

<sup>2</sup> Web Dev Simplified. “Build A REST API With Node.js, Express, & MongoDB - Quick” YouTube, May 14 2019, https://www.youtube.com/watch?v=IYvD9oBCuJI.