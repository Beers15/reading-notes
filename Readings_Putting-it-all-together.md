[Home](README.md)

# Readings: Putting it all together

### React Docs - Thinking in React
---------------

Referenced the source below for answers<sup>1<sup>


1. How would you break a mock into a component heirarchy?

  
* Create a diagram with every component within your application. Applying the single resposibility priniciple can help you determine if something should be considered a component   that will be applied to your diagram. Drawing your UI and denoting each individual component is a good way to accomplish this as well.


2. What is the single responsibility principle and how does it apply to components?

  
* A component should only have a single purpose. If your component ends up taking on more than one task, break it up into multiple components.

  
3. What does it mean to build a ‘static’ version of your application?

  
* This can be done by building a version of your app that reuses components that you've created. Pass props as needed and ignore state in the static version of your app since the static version doesn't need interactivity.

  
4. Once you have a static application, what do you need to add?

  
* Once the static version of your application is complete, you can implement state to make your app interactive. Minimize state as much as possible.

  
5. What are the three questions you can ask to determine if something is state?

  
* As per the official React documentation, to determine if something is state ask these questions:

  
  "Is it passed in from a parent via props? If so, it probably isn’t state.
  Does it remain unchanged over time? If so, it probably isn’t state.
  Can you compute it based on any other state or props in your component? If so, it isn’t state."<sup>1<sup>



6. How can you identify where state needs to live?

* As per the official React documentation, to identify where state needs to live take the following steps:

  "Identify every component that renders something based on that state.
  Find a common owner component (a single component above all the components that need the state in the hierarchy).
  Either the common owner or another component higher up in the hierarchy should own the state.
  If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common   owner component."<sup>1<sup>


## Things I want to know more about
---------------
* Although the steps in the article below serve as a good set of guidlines for creating an app, I would want to know more abou this process through additional tutorials and examples.

###### Works Cited
<sup>1</sup> _Thinking in React_, React, https://reactjs.org/docs/thinking-in-react.html Accessed 19 Aug 2021.
