[Home](README.md)
 
# Readings: Authentication
 
## Review, Research, and Discussion
 
---------------
 
Referenced cited article below for answers<sup>1</sup>
 
1) Explain what a “Singleton” is (in Computer Science terms)
 
    This is when a module exports a lone instance of a itself, as only one instance of it is really needed. (e.g. the app object in Express that represents your server)
 
2) Explain how the Singleton pattern can be used with Node modules, specifically with classes
 
    It can be used to only allow a single instance of a class to be created.
    The code snippet below shows a strategy where a paired class checks to see if there is already an instance of a singleton class, and creates one if not. Only one instance can be created. By exporting a singleton object that wraps the main object, only one instance will ever be exported from the node module.

    <sup>1</sup>

    ```
      class Logger {
        constructor() {
            this.logs = [];
        }
        get count() {
            return this.logs.length;
        }
        log(message) {
            const timestamp = new Date().toISOString();
            this.logs.push({ message, timestamp });
            console.log(`${timestamp} - ${message}`);
        }
      }

      class Singleton {
        constructor() {
            if (!Singleton.instance) {
                Singleton.instance = new Logger();
            }
        }
        getInstance() {
            return Singleton.instance;
        }
      }

      module.exports = Singleton;

    ```
 
3) If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
 
    This is a complicated task, so my approach would be to try to make my system as close to Express as possible. I would use a singleton to represent my server. I would push any  middleware functions into a collection within my server object. Whenever any requests were made, I would iterate through this collection. Only when a function similar to Express' 'next' would the system procced to the next function, passing values reperesenting errors if any. Etc, etc...
 
### Vocabulary terms
 
Router Middleware

  * This middleware is more specific than app-level middleware in that it applies to a specific express router object.

Dynamic Module Loading

  * I believe this is when you use a 3rd party library, or define one, that has a space with various modules contained in it. As modules are needed and used, they are loading in for use. Modules refernced in this space are not defined explicitly and are not loaded into the program beforehand.

Singleton Pattern <sup>1</sup>

  * A design pattern where your program only needs a lone instance of a particular object to be created.

CRUD -> REST Method Matches

  * Create, read, update, delete -> Rest Equivalents: POST, GET, POST/PATCH, DELETE 

Mock Testing <sup>2</sup>

  * This is a type a testing where a fake version of a service is created and tests are done against this fake instead of the actual service. The benefit of this is that tests can be more controlled, reliable, and quick (e.g. using the supertest library to mock an instance of an express app to conduct unit tests).

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
 
    Different types of attacks hackers will try to try to overcome hashing encryption protection

    What the Authorization header is used for

    Encryption with the Bcrypt module

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
 
    How to utilize Bcrypt library to create 'air-tight' security when defining authorization and authentication data flows

    Creating secure apps that follow the guidelines the OWASP defines 

    Commonly used libraries that abstract a lot of the authorization and authentication covered in the readings into an easier to use format
 
3) What are you most excited about trying to implement or see how it works?
 
    Defining authorization and authentication middleware
 
#### Works Cited
 
<sup>1</sup>Kumawat, Mahesh, _Node.js Design Patterns — Singleton pattern ( Series -1)_, Medium, Apr 30, 2018, https://medium.com/@maheshkumawat_83392/node-js-design-patterns-singleton-pattern-series-1-1e0ab71e3edf

<sup>2</sup>Jung, June, _How to test software, part I: mocking, stubbing, and contract testing_, circleci Blog, Apr 4, 2019, https://circleci.com/blog/how-to-test-software-part-i-mocking-stubbing-and-contract-testing/
