[Home](README.md)
 
# Readings: Data Modeling
 
## Review, Research, and Discussion
 
---------------
 
1) Name 3 advantages to Test Driven Development
 
    TDD helps prevent bugs in your code. It helps give the developer well placed confidence that their app works well. When integrated with CI/CD, good TDD ensures the code pushed to a production environment is ready for user consumption.
 
2) In what case would you need to use beforeEach() or afterEach() in a test suite?
 
    It may be useful to call these methods when you are testing database operations and need to sanitize the db between individual unit tests.
 
3) What is one downside of Test Driven Development
 
    It's slow! It could be a hindrance instead of a boon when writing smaller applications.
 
4) What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
 
    This would be the syntax. They accomplish the same tasks. ES6 classes are just a syntactically more pleasing version of Constructor/Prototype Classes.
 
5) Why REST?
 
    It's easier to use than other methods of dealing with resources on the web such as SOAP. REST operations are easy to understand and have clear meanings. Resources in this architecture are easy to identify as well. REST APIs are stateless, which makes them easier to scale. <sup>1</sup>
 
### Vocabulary terms
 
* functional programming

  This is a programming paradigm where the aim is to write pure functions and take a declarative approach when programming instead of an imperative one.
 
* Objected-oriented programming

  This is a programming paradigm that revolves around creating classes that can be used to instantiate bundles of related logic and data, or objects.
 
* class
 
  A class is a data structure that defines attributes and behaviors to create a blueprint for the objects that can be instantiated from it.
 
* super
 
  A keyword that can be used to refer to the superclass to call superclass methods/properties from the subclass
 
* this
   
  The this keyword is a reference to an object that it is binded to. 

* Test Driven Development (TDD)

  This is a development style were all features of an application are incrementally developed with test cases ensure they work.
 
 
### Preview
 
 
1) Which 3 things had you heard about previously and now have better clarity on?
 
    The strengths of both SQL and NoSQL DBs, application types that would benefit from an SQL DB vs ones that would benefit from a NoSQL DB, and how to mock up tables and their  relationships in a relational DB
 
2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
 
    Mocking tables and their relationships to other tables, how to define different types of relationships (1-1, 1-many, etc) using Sequelize, and how to query tables that have relationships with other tables and populate the data from what they are related to
 
3) What are you most excited about trying to implement or see how it works?
 
    Add data validation/constraints to the columns in a SQL table
 
#### Works Cited
 
<sup>1</sup>ServiceObjects, _Why REST is Becoming so Popular_, https://www.serviceobjects.com/articles-whitepapers/why-rest-popular/
