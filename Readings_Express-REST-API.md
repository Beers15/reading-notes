[Home](README.md)
 
# Readings: Express REST API
 
## Review, Research, and Discussion
 
---------------
 
Referenced express docs for answers<sup>1</sup>
 
1) Name 3 real world use cases where you’d want to change the request with custom middleware<sup>2</sup>
 
    * You could add to the request body the date that it was submitted to your express server.
 
    * If for some reason you wanted to change a request method from one type to another you could do so with middleware.
 
    * You could change the headers of your req object.
 
2) True or false: The route handler is middleware?
 
    False, the route handler is always called on a specific route and does not need to be called. However, if there are more than 1 function in a route definition, all but the last fnc are middleware fncs.
 
3) In what ways can a middleware function end the process and send data to the browser?
 
    Middleware has access to the request and response objects used by express. By calling res.send, res.render, or res.redirect a middleware fnc can send data to the browser.
 
4) At what point in the request lifecycle can you “inject” middleware?
 
    Middleware can be injected immediately after the request is made or any point after until a response is sent.
 
5) What can cause express to error with “Request headers sent twice, cannot start a second response”
 
    I've personally encountered this error when returning a response with res.send and forgetting to return or break execution before another res.send is executed.
 
### Vocabulary terms
 
Referenced express docs for answers<sup>1</sup>
 
* Middleware
  In Express middleware are fncs that execute during the WRRC. In other words, they are fncs that execute after the request is made and before the response is sent.
 
* Request Object
 
  This is an object representing the incoming request in an Express app.
 
* Response Object
 
  This is an object representing the outgoing response in an Express app.
 
* Application Middleware
 
  This is middleware configured with app.use and no optional path argument. The middleware will apply to every request and will be chained in order depending on where it's defined.
 
* Routing Middleware
 
  This is middleware that is supplied to a specific route. It will only be executed on that route and will be chained in order depending on where it's passed in to the route.
 
* Test Driven Development
 
  This is a style of development where unit testing takes place before or in conjunction with feature development. Tests are incrementally created as new features are added to ensure good working code.
 
* Behavioral Testing <sup>3</sup>
 
  This kind of testing is centered around the user and the actions they would take on your web application instead of individual units. It's more oftenly used to get a business point of view across instead of a more technical one.
 
### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
 
    Middleware, TDD, and route handlers
 
2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
 
    Working with classes JS, advanced routing in Express apps, working more with Postgres
 
3) What are you most excited about trying to implement or see how it works?
 
    Using Sequelize + SQL for our model layer instead of mongoose + MongodB
 
#### Works Cited
 
<sup>1</sup>Express, _Using middleware_, https://expressjs.com/en/guide/using-middleware.html
 
<sup>2</sup>Le, William, _How To Use the req Object in Express_, Digitalocean, Dec 24 2020, https://www.digitalocean.com/community/tutorials/nodejs-req-object-in-expressjs
 
<sup>3</sup>Katalon, _Behavior Driven Testing in Automated testing_, https://www.katalon.com/sa/behavior-driven-testing/
