[Home](README.md)
 
# Readings: React Native
 
## Review, Research, and Discussion
 
---------------
Answers taken in part from resources listed below

1) Compare and Contrast Redux Toolkit with Redux “Ducks”

  * Ducks is a pattern that is sometimes recommended to be followed when implementing larger Redux applications in order to keep them highly modular and very scalable. This pattern is often implemented with Redux toolkit. Whether it used with the toolkit or not, the idea is that all redux logic (actions, action creators, state, reducers) related to a single feature of an app should be contained in a 'slice'. Redux Toolkit always uses slices by default.

2) What is the principle advantage of Redux Toolkit

  * It provides an implementation of the Redux store that has less boilerplate code, less complexity, and has redux-thunk built in. 


### Vocabulary terms

redux toolkit slices

  * This is a higher order function that inits the state and reducer for a resource, similar to a vanilla Redux reducer. Unlike a redux reducer, it also generates the related actions + actions creators automatically.

namespace

  * This is a defined scope for identifiers. Functions, variables, etc with the same name can cause issues when they are needed in the same context unless they are contained in different namespaces. 

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    * React-Native
    * Redux-toolkit
    * namespaces

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * The various components that come with React-Native out of the box
    * How to better use Expo with VS code
    * How to effectively use the Redux-Ducks pattern
 
3) What are you most excited about trying to implement or see how it works?
 
    * Creating React-Native applications that I can use on my android devices

--------------

### Resources

https://www.geeksforgeeks.org/javascript-namespace/

https://reactnative.dev/docs/getting-started

https://reactnative.dev/docs/tutorial

https://redux.js.org/style-guide/style-guide

https://reactnative.dev/

https://expo.dev/

https://snack.expo.dev/

https://docs.expo.dev/versions/latest/expokit/eject