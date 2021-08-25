[Home](README.md)

# Readings: APIs

### API Design Best Practices
---------------
Referenced the source below for answers<sup>1<sup>

1. What does REST stand for?

  Representational State Transfer

2. REST APIs are designed around a *resources*.


3. What is an identifer of a resource? Give an example.

  This is a URI (universal resource indentifier). For example, these often follow a format like https://somesite.com/route/id


4. What are the most common HTTP verbs?

  These are GET, POST, PUT, PATCH, DELETE


5. What should the URIs be based on?

  "When possible, resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource)."<sup>1</sup>


6. Give an example of a good URI.

  https://www.someredditclone.com/posts/


7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

  This is when a web API exposes many resources. This is bad since it results in more requests when fetching the needed data.


8. What status code does a successful GET request return?

  The 200 status code (OK)

9. What status code does an unsuccessful GET request return?

  Depends on the error. In the case that the resource can not be found the 404 status code (Not Found) is returned.


10. What status code does a successful POST request return?

  The 201 status code (created)


11. What status code does a successful DELETE request return?

  The 204 status code (No Content)


### REGEXP
---------------
Referenced the source below for answer<sup>2<sup>

1. How would you match your name using RegEx. 
This would be one of many possible matches /[^A][\w]{7}[\s][\w]{4}[$s]/


## Things I want to know more about
---------------
  * What regexps could be used for partial matches with search utilities. (Similar to the LIKE operater in sql, or a good fuzzy search)
  * Creating APIs that can handle the various REST request types
  * HTTP headers


###### Works Cited 
---------------
<sup>1</sup> Microsoft, _RESTful web API design_, Jan 12 2018, https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design

<sup>2</sup> Fox, Jonny _Regex tutorial - A quick cheatsheet by examples_, Factory Mind, Medium, 22 Jun 2017, https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285




###### Works Cited

<sup>1</sup>https://gist.github.com/brookr/5977550