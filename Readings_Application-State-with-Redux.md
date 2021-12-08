[Home](README.md)
 
# Readings: API Integration
 
## Review, Research, and Discussion
 
---------------
All answers taken from the resources below

1) What are the advantages of storing tokens in “Cookies” vs “Local Storage”

  * Cookies are usable by a server while local storage is client side. Local storage is easy to use, but more vulnerable to security attacks. Cookies on the other hand are a bit more secure, but have a very small size limit of 4kb. Given these considerations, with sensitive data and/or tokens it may be better to use cookies. Local storage may be better otherwise. 

2) Explain 3rd party cookies.

  * These are cookies that are sent to your browser by sites other than the one that you currently are on.

3) How do pixel tags work?

  * Pixel tags represent an element on a webpage and contains all sorts of information on that element. They are often used by sites to obtain information about the user browsing a webpage. This information is used to create (often unwanted) cookies that are sent to the users browser and perform other actions such as tracking (e.g. add servers read pixel tags from the pages you visit to tailor adds for you).

### Vocabulary terms

cookies

  * Cookies are bits of data that are sent as a part of an HTTP request and response created by a server. They are stored in the browser. 

authorization

  * Ensuring an entity has permission to perform a certain action or access a given resource that is secure

access control

  * A security technique where certain actions or resources are only able to be performed by those who are given permission by a the given system 

conditional rendering

  * The showing or hiding of various UI components based on the value of some state

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?

    * Redux
    * Reducers
    * Actions

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Testing React Applications that use redux to manage global state
    * Integrating Redux into react apps
    * Using HTTP cookies
 
3) What are you most excited about trying to implement or see how it works?
 
    * Creating large scale React apps where Redux's configuration complexity ends up being well worth it

--------------

### Resources

https://learnwebanalytics.com/whats-the-difference-between-a-cookie-a-pixel-and-a-tag/

https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867

https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6/

https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1

https://redux.js.org/

https://www.cookiepro.com/knowledge/what-is-a-third-party-cookie/

https://dev.to/cotter/localstorage-vs-cookies-all-you-need-to-know-about-storing-jwt-tokens-securely-in-the-front-end-15id